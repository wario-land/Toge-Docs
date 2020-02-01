### Tileset indices

The game stores the tileset index of the current map at the RAM location 0x03000074. It uses it calculate the tileset record offset below.

| ID   | Description
| -----|------------
| 0x00 | Debug room
| 0x01 | Palm Tree Paradise
| 0x02 | Caves
| 0x03 | The Big Board
| 0x04 | The Big Board
| 0x05 | The Big Board?
| 0x06 | Wildflower Fields
| 0x07 | Toy Block Tower
| 0x08 | The Curious Factory
| 0x09 | Wildflower Underground?
| 0x0A | Wildflower/Jungle?
| 0x0B | Underwater?
| 0x0C | Toy Block Tower
| 0x0D | Toy Block Tower
| 0x0E | Toy Block Tower (purple)
| 0x0F | Doodle Woods
| 0x10 | Domino Row
| 0x11 | Hall of Hieroglyphs
| 0x12 | Haunte House? (plus debug tiles)
| 0x13 | Crescent Moon Village (outside)
| 0x14 | Haunted House?
| 0x15 | Arabian Night (outside)
| 0x16 | Arabian Night (inside)
| 0x17 | Arabian Night
| 0x18 | Arabian Night
| 0x19 | Arabian Night
| 0x1A | Domino Row (blue)
| 0x1B | Domino Row (purple)
| 0x1C | Domino Row (teal)
| 0x1D | The Curious Factory
| 0x1E | The Curious Factory
| 0x1F | Jungle
| 0x20 | The Curious Factory
| 0x21 | The Toxic Landfill
| 0x22 | The Toxic Landfill
| 0x23 | Pinball Zone
| 0x24 | Pinball Zone
| 0x25 | Pinball Zone (with Gorilla)
| 0x26 | Jungle
| 0x27 | 40 Below Fridge?
| 0x28 | Jungle
| 0x29 | Jungle caves
| 0x2A | Hotel Horror
| 0x2B | Hotel Horror
| 0x2C | Hotel Horror
| 0x2D | Hotel Horror
| 0x2E | Hotel Horror
| 0x2F | Hotel Horror (outside)
| 0x30 | Unused in-game (Haunted House)
| 0x31 | Unused in-game (Haunted House)
| 0x32 | Unused in-game (Cardboard)
| 0x33 | Cardboard
| 0x34 | Caves
| 0x35 | Jungle
| 0x36 | Caves
| 0x37 | Fiery Cavern (lava)
| 0x38 | Caves
| 0x39 | Golden Passage
| 0x3A | Hotel Horror
| 0x3B | Hotel Horror
| 0x3C | Hotel Horror
| 0x3D | Hotel Horror
| 0x3E | 40 Below Fridge
| 0x3F | The Curious Factory
| 0x40 | The Curious Factory
| 0x41 | Arabian Night
| 0x42 | Arabian Night?
| 0x43 | Boss corridor
| 0x44 | Boss room? (golden)
| 0x45 | Fiery Cavern (frozen)
| 0x46 | Lava level
| 0x47 | Hall of Hieroglyphs
| 0x48 | Boss room?
| 0x49 | Boss room?
| 0x4A | Boss corridor
| 0x4B | Boss corridor
| 0x4C | Boss corridor
| 0x4D | Boss corridor
| 0x4E | Boss corridor
| 0x4F | Boss room?
| 0x50 | Hall of Hieroglyphs
| 0x51 | Jungle
| 0x52 | Wildflower Fields
| 0x53 | Crescent Moon Village
| 0x54 | Crescent Moon Village
| 0x55 | Crescent Moon Village
| 0x56 | Toy Block Tower
| 0x57 | Pinball Zone
| 0x58 | Bonus room
| 0x59 | Bonus room
| 0x5A | Final level
| 0x5B | The Big Board (end)

### Tileset header table

Each tileset index indexes a record in a global tileset record table starting from `0x083F2298`. The record are 36 bytes long. There are 92 records in the table.

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u32_ptr   | Pointer to foreground graphics
| +0x04  | u32       | (?) Some data (migh be some data size)
| +0x08  | u32_ptr   | Pointer to palette
| +0x0C  | u32_ptr   | Pointer to background graphics
| +0x10  | u32       | (?) Some data (migh be some data size)
| +0x14  | u32_ptr   | (?) Pointer
| +0x18  | u32_ptr   | (?) Pointer
| +0x1C  | u32_ptr   | (?) Pointer
| +0x20  | u32_ptr   | (?) Pointer

TODO: List unused records.
