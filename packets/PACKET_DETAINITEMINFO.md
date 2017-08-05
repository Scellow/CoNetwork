**MsgDetainItemInfo:** This packet is sent to fill the detained items window.

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira/|Felipe Vieira]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 112 |
| 2 | UINT16 | Packet Identifier | 10014 |
| 4 | UINT32 | Detain Identity | 103 |
| 8 | UINT32 | Item Identity | 54646 |
| 12 | UINT32 | Item Type | 410339 |
| 16 | UINT16 | Durability | 7099 |
| 18 | UINT16 | Maximum Durability | 7099 |
| 20 | UINT16 | Detain Mode | 1 |
| 24 | UINT32 | Socket Progress | 1000 |
| 28 | BYTE | Socket One | 13 |
| 29 | BYTE | Socket Two | 13 |
| 30 | BYTE | Item Effect | 200 |
| 32 | BYTE | Plus | 12 |
| 33 | BYTE | Blessing | 7 |
| 34 | BYTE | Bound | 0 |
| 35 | BYTE | Enchantment | 252 |
| 40 | BYTE | Suspicious | 0 |
| 42 | BYTE | Locked | 0 |
| 44 | BYTE | Item Color | 3 |
| 48 | UINT32 | Character Identity | 1000002 |
| 52 | STRING | Character Name | Length16String12 |
| 68 | UINT32 | Target Identity | 1000003 |
| 72 | STRING | Target Name | szHunterOrTarget |
| 88 | UINT32 | Capture Date | 20161001 |
| 96 | UINT32 | CPs Cost | 1950 |
| 100 | BYTE | Expired | 1 |
| 108 | UINT | Days Left | 6 |

**Note:** The character name is the player who is viewing the item and the target is the hunter or who lost the equip.
