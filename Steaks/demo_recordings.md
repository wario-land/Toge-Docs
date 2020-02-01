# Demo recordings

## Demo orderlist

* Starts at: 0x0840092C
* Record count: 16
* Record type: u8

This list determines in which order the demos recordings are played. The game stores the index of the currently played orderlist index at the location 0x03000020.

## Demo recording headers

* Starts at: 0x0840086C
* Record count: 16
* Record length: 12 bytes

| Index | Demo level
| ----- | ----------
| 0x00  | Hall of Hieroglyphs
| 0x01  | Palm Tree Paradise
| 0x02  | Wildflower Fields
| 0x03  | Mystic Lake
| 0x04  | Monsoon Jungle
| 0x05  | Cractus
| 0x06  | The Curious Factory
| 0x07  | 40 Below Fridge
| 0x08  | Pinball Zone
| 0x09  | Aerodent
| 0x0A  | Toy Block Tower
| 0x0B  | Doodle Woods
| 0x0C  | Domino Row
| 0x0D  | Arabian Night
| 0x0E  | Fiery Cavern
| 0x0F  | Hotel Horror

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u8        | Passage index
| +0x01  | u8        | Stage index
| +0x02  | u8        | Area index
| +0x03  | u8        | Padding
| +0x04  | u16       | Starting X-position in the area
| +0x06  | u16       | Starting Y-position in the area
| +0x08  | u16       | Background music index
| +0x0A  | u16       | Padding

## Pointer tables

These tables are indexed by the demo header index.

| Offset     | Count  | Description
| ---------- | ------ | -----------
| 0x0878F5F4 | 0x10   | Button states
| 0x0878F634 | 0x10   | Timings

## Data format and playback

The button states and timings are both defined as u16 arrays. The button state data copied to 0x03002CC8, the timings are copied to 0x03002EC8 for playback. The timings might be given in frames.

| Value  | Button
| -------| ------
| 0x0001 | A
| 0x0002 | B
| 0x0004 | (?)
| 0x0008 | (?)
| 0x0010 | Right
| 0x0020 | Left
| 0x0040 | Up
| 0x0080 | Down
| 0x0100 | (?)
| ...    | ...
