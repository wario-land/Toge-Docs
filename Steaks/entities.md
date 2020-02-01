# Entities

## Entity lists

The entities for each area and difficulty level stored in separate lists. A record containing all 0xFF fields marks the end of the list.

| Offset | Data type | Description
| ------ | --------- | -----------
| +0x00  | u8        | Y-coordinate (top -> bottom)
| +0x01  | u8        | X-coordinate (left -> right)
| +0x02  | u8        | Entity index

## Entity indices

It seems like every map has a local selection of entities from a global list. Entities below 0x10 seems to be shared between every map.

| Index | Entity
| ----- | ------
| 0x00  | Game crash
| 0x01  | Box with top-right quadrant
| 0x02  | Box with bottom-right quadrant
| 0x03  | Box with bottom-left quadrant
| 0x04  | Box with top-left quadrant
| 0x05  | CD box
| 0x06  | Health box
| 0x07  | Large diamond
| 0x08  | Frog switch
| 0x09  | Keyzer
| 0x10  | Black cat
| 0x11  | Portal
| 0x12  | Walking torch
| 0x13  | Totsumen
| 0x14  | Rock to throw
| 0x15  | Opened box
