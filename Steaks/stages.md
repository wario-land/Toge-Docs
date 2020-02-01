# Stages

## Stage header indices

- Starts at: 0x086391C4
- Record count: 36
- Record type: u32

| Index | Offset     | Description
| ----- | ---------- | -----------
| 0x00  | 0x086391C4 | Hall of Hieroglyphs
| 0x01  | 0x086391C8 | *Null*
| 0x02  | 0x086391CC | Debug Stage
| 0x03  | 0x086391D0 | *Null*
| 0x04  | 0x086391D4 | Spoiled Rotten
| 0x05  | 0x086391D8 | Mini-Game Shop
| 0x06  | 0x086391DC | Palm Tree Paradise
| 0x07  | 0x086391E0 | Wildflower Fields
| 0x08  | 0x086391E4 | Mystic Lake
| 0x09  | 0x086391E8 | Monsoon Jungle
| 0x0A  | 0x086391EC | Cractus
| 0x0B  | 0x086391F0 | Mini-Game Shop
| 0x0C  | 0x086391F4 | The Curious Factory
| 0x0D  | 0x086391F8 | The Toxic Landfill
| 0x0E  | 0x086391FC | Pinball Zone
| 0x0F  | 0x08639200 | 40 Below Fridge
| 0x10  | 0x08639204 | Cuckoo Condor
| 0x11  | 0x08639208 | Mini-Game Shop
| 0x12  | 0x0863920C | Toy Block Tower
| 0x13  | 0x08639210 | The Big Board
| 0x14  | 0x08639214 | Doodle Woods
| 0x15  | 0x08639218 | Domino Row
| 0x16  | 0x0863921C | Aerodent
| 0x17  | 0x08639220 | Mini-Game Shop
| 0x18  | 0x08639224 | Crescent Moon Village
| 0x19  | 0x08639228 | Arabian Night
| 0x1A  | 0x0863922C | Fiery Cavern
| 0x1B  | 0x08639230 | Hotel Horror
| 0x1C  | 0x08639234 | Catbat
| 0x1D  | 0x08639238 | Mini-Game Shop
| 0x1E  | 0x0863923C | Golden Passage
| 0x1F  | 0x08639240 | *Null*
| 0x20  | 0x08639244 | *Null*
| 0x21  | 0x08639248 | *Null*
| 0x22  | 0x0863924C | Golden Diva
| 0x23  | 0x08639250 | Mini-Game Shop

## Stage headers

- Starts at: 0x08639068
- Record count: 29
- Record length: 12 bytes

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u8        | Area header pointer index
| +0x01  | u8        | Area count
| +0x02  | u8        | Always 0x0A
| +0x03  | u24       | Hard mode time limit
| +0x06  | u24       | Normal mode time limit
| +0x09  | u24       | S-Hard mode time limit

| Index | Offset     | Description
| ----- | ---------- | -----------
| 0x00  | 0x08639068 | Hall of Hieroglyphs
| 0x01  | 0x08639074 | Palm Tree Paradise
| 0x02  | 0x08639080 | Wildflower Fields
| 0x03  | 0x0863908C | Mystic Lake
| 0x04  | 0x08639098 | Monsoon Jungle
| 0x05  | 0x086390A4 | Cractus
| 0x06  | 0x086390B0 | Mini-Game Shop
| 0x07  | 0x086390BC | The Curious Factory
| 0x08  | 0x086390C8 | The Toxic Landfill
| 0x09  | 0x086390D4 | Pinball Zone
| 0x0A  | 0x086390E0 | 40 Below Fridge
| 0x0B  | 0x086390EC | Cuckoo Condor
| 0x0C  | 0x086390F8 | Mini-Game Shop
| 0x0D  | 0x08639104 | Toy Block Tower
| 0x0E  | 0x08639110 | The Big Board
| 0x0F  | 0x0863911C | Doodle Woods
| 0x10  | 0x08639128 | Domino Row
| 0x11  | 0x08639134 | Aerodent
| 0x12  | 0x08639140 | Mini-Game Shop
| 0x13  | 0x0863914C | Crescent Moon Village
| 0x14  | 0x08639158 | Arabian Night
| 0x15  | 0x08639164 | Fiery Cavern
| 0x16  | 0x08639170 | Hotel Horror
| 0x17  | 0x0863917C | Catbat
| 0x18  | 0x08639188 | Mini-Game Shop
| 0x19  | 0x08639194 | Golden Diva
| 0x1A  | 0x086391A0 | Spoiled Rotten
| 0x1B  | 0x086391AC | Debug Stage
| 0x1C  | 0x086391B8 | Golden Passage

## Area header pointers

- Starts at: 0x0878F280
- Record count: 25
- Record type: u32_ptr

| Index | Offset     | Description
| ----- | ---------- | -----------
| 0x00  | 0x0878F280 | Hall of Hieroglyphs
| 0x01  | 0x0878F284 | Palm Tree Paradise
| 0x02  | 0x0878F288 | Wildflower Fields
| 0x03  | 0x0878F28C | Mystic Lake
| 0x04  | 0x0878F290 | Monsoon Jungle
| 0x05  | 0x0878F294 | The Curious Factory
| 0x06  | 0x0878F298 | The Toxic Landfill
| 0x07  | 0x0878F29C | Pinball Zone
| 0x08  | 0x0878F2A0 | 40 Below Fridge
| 0x09  | 0x0878F2A4 | Toy Block Tower
| 0x0A  | 0x0878F2A8 | The Big Board
| 0x0B  | 0x0878F2AC | Doodle Woods
| 0x0C  | 0x0878F2B0 | Domino Row
| 0x0D  | 0x0878F2B4 | Crescent Moon Village
| 0x0E  | 0x0878F2B8 | Arabian Night
| 0x0F  | 0x0878F2BC | Hotel Horror
| 0x10  | 0x0878F2C0 | Fiery Cavern
| 0x11  | 0x0878F2C4 | Cractus
| 0x12  | 0x0878F2C8 | Cuckoo Condor
| 0x13  | 0x0878F2CC | Aerodent
| 0x14  | 0x0878F2D0 | Catbat
| 0x15  | 0x0878F2D4 | Golden Diva
| 0x16  | 0x0878F2D8 | Spoiled Rotten
| 0x17  | 0x0878F2DC | Golden Passage
| 0x18  | 0x0878F2E0 | Debug Stage

## Area headers

- Starts at: 0x083F4E88
- Record count: 242
- Record length: 44 bytes

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u8        | Tileset index
| +0x01  | u8        | Layer 0 properties
| +0x02  | u8        | Layer 1 properties
| +0x03  | u8        | Layer 2 properties
| +0x04  | u8        | Layer 3 properties
| +0x05  | u24       | Padding
| +0x08  | u32_ptr   | Layer 0 data
| +0x0C  | u32_ptr   | Layer 1 data
| +0x10  | u32_ptr   | Layer 2 data
| +0x14  | u32_ptr   | Layer 3 data
| +0x18  | u8        | (?) Layer priority
| +0x19  | u8        | (?) Layer priority
| +0x1A  | u8        | (?) Layer priority
| +0x1B  | u8        | (?) Layer priority / (?) Padding
| +0x1C  | u32_ptr   | Hard mode entities
| +0x20  | u32_ptr   | Normal mode entities
| +0x24  | u32_ptr   | S-Hard mode entities
| +0x28  | u8        | (?)
| +0x29  | u8        | (?)
| +0x2A  | u8        | (?)
| +0x2B  | u8        | (?)

## Warp list pointers

- Starts at: 0x0878F21C
- Record count: 25
- Record type: u32_ptr

| Index | Offset     | Description
| ----- | ---------- | -----
| 0x00  | 0x0878F21C | Hall of Hieroglyphs
| 0x01  | 0x0878F220 | Palm Tree Paradise
| 0x02  | 0x0878F224 | Wildflower Fields
| 0x03  | 0x0878F228 | Mystic Lake
| 0x04  | 0x0878F22C | Monsoon Jungle
| 0x05  | 0x0878F230 | The Curious Factory
| 0x06  | 0x0878F234 | The Toxic Landfill
| 0x07  | 0x0878F238 | Pinball Zone
| 0x08  | 0x0878F23C | 40 Below Fridge
| 0x09  | 0x0878F240 | Toy Block Tower
| 0x0A  | 0x0878F244 | The Big Board
| 0x0B  | 0x0878F248 | Doodle Woods
| 0x0C  | 0x0878F24C | Domino Row
| 0x0D  | 0x0878F250 | Crescent Moon Village
| 0x0E  | 0x0878F254 | Arabian Night
| 0x0F  | 0x0878F258 | Hotel Horror
| 0x10  | 0x0878F25C | Fiery Cavern
| 0x11  | 0x0878F260 | (?) Cractus
| 0x12  | 0x0878F264 | (?) Cuckoo Condor
| 0x13  | 0x0878F268 | (?) Aerodent
| 0x14  | 0x0878F26C | (?) Catbat
| 0x15  | 0x0878F270 | (?) Golden Diva
| 0x16  | 0x0878F274 | (?) Spoiled Rotten
| 0x17  | 0x0878F278 | (?) Golden Passage
| 0x18  | 0x0878F27C | (?) Debug stage

## Warps

- Starts at: 0x083F2F88
- Record count: 660
- Record length: 12 bytes

Records filled with zeroes separates stages.

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u8        | (?) Warp type: 0x00 - End of list, 0x01 - Vortex, 0x02 - Side of screen, 0x03 - Pipe, 0x04 - (?), 0x05 - (?)
| +0x01  | u8        | Area index
| +0x02  | u8        | (?) X-coordinate when it's source/target
| +0x03  | u8        | (?) X-coordinate when it's target/source
| +0x04  | u8        | (?) Y-coordinate when it's source/target
| +0x05  | u8        | (?) Y-coordinate when it's target/source
| +0x06  | u8        | Target warp index (0x00 - Stage select screen)
| +0x07  | u8        | (?) Possible values: 0x00, 0x08, 0x18, 0x20, 0x24, 0x40, 0xE0, ...
| +0x08  | u8        | (?) Similar to the previous value
| +0x09  | u8        | (?) Connected somehow to entities
| +0x0A  | u16       | Music index (0x0000 - No change)

## TODO

* Area headers at 0x02000000
* Decompressed area data at 0x02000040
* Area destruction list at 0x0203A000

<!--
### Layer settings

TODO:
0x00-Disabled
0x10-Enabled with collisions
0x11-Enabled without collision

### Map compression

TODO: RLE, not the BIOS RLE one

### Foreground layer data

TODO: w:u8, h:u8, rle_stream

### Background layer data

TODO: size:u8, rle_stream (1024/2048 bytes after decompression)
-->
