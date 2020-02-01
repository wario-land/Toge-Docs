# Wario Land 4 ROM Hacking Docs

## About this document

This document contains information about the data structures and algorithms used by a game called Wario Land 4. The goal of this document is to aid my process developing *Steaks!*, a level editor for the game. This document is work in progress, it's incomplete and some of its statements might be incorrect.

### Pointers for yet unknown map related things

They start from 0x0878F540, 25 pointers (same order as the previous pointers). I have no idea where they point to but it's somehow related to the camera or the map scrolling.

## Entering the debug mode in-game

This disassembled code below suggests that it might be possible to activate the debug mode inside the game without any memory poking or emulator cheat codes. I have yet no idea how.

```
08079CB4 4903     ldr     r1,=#0x3000C3C
08079CB6 2008     mov     r0,#0x8
08079CB8 E328     b       #0x807A30C
...

08079CDC 4903     ldr     r1,=#0x3000C3C
08079CDE 2008     mov     r0,#0x8
08079CE0 E314     b       #0x807A30C
...

08079D04 4903     ldr     r1,=#0x3000C3C
08079D06 2008     mov     r0,#0x8
08079D08 E300     b       #0x807A30C
...

08079D2C 4903     ldr     r1,=#0x3000C3C
08079D2E 2008     mov     r0,#0x8
08079D30 E2EC     b       #0x807A30C
...

0807A30C 8008     strh    r0,[r1]  ; <- Here sets the debug mode
0807A30E 8820     ldrh    r0,[r4]
0807A310 4328     orr     r0,r5
0807A312 8020     strh    r0,[r4]
0807A314 E029     b       #0x807A36A
...

0807A36A F000FCB7 bl      #0x807ACDC
...
```

The following code turns **off** the debug mode:

```
0801D32C 4816     ldr     r0,=#0x3000C3C
0801D32E 2102     mov     r1,#0x2
0801D330 8001     strh    r1,[r0]
```

## Interesting things I found

- In the Hall of Hieroglyphs stage the piping section might have been added at late development. Proof: The map IDs are 4-15-16-5-6-7-8-9-10-11-12-13-14.
- The Hotel Horror stage may preceeded the Fiery Cavern stage. In the ROM it always does.

# TODOs
- Passage destinations: 0x086391C4 + (i * 4), Values: 0x00-0x1C
- Another passage destination map: 0x08639068 + (i * 12), First byte: destination stage index
- Overworld passage connections: 0x086392D0 + (i * 4), values starting from 0x00: Entry, Emerald, Ruby, Topaz, Sapphire, Pyramid, Sound Room,
- Starting from 0x083F7828 there are (u32, gfx pointer) pairs. Have no idea what they do.
- Collectible appearances (?) -> 16 x u16 per map, for HoH screen 3 starts at 0x083F8978
- Starting from 0x083B14F0 there are 32 bytes long records. Connected somehow to the entities.
- Starting from 0x0878F714 there are around 90 pointers what sdefines what kind of particles are created when something is collected or broken.
- Starting from 0x0x78F5A4 there are around 20 pointers what might define tile property like things (ability to break and collect things, etc.).
- Pointers at 0x0863A43C: might be connected to passages/stages somehow
- from 0x0878E780 to 0x0878F970 there are several of pointers to warps
