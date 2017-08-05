**MsgItemInfo:** This packet is sent server>client to add or update the attributes of a specific item.

**Patch 5017:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 44|
| 2 | UINT16 | Packet Identifier | 1008|
| 4 | UINT32 | UniqueID | 1 |
| 8 | UINT32 | StaticID | 730001 |
| 12 | UINT16 | Durability | 10000 |
| 14 | UINT16 | MaxDurability | 10000 |
| 16 | UINT16 | [[msgiteminfoaction|Action Type]]| 1 |
| 18 | Byte | Location| 0 |
| 19 | Byte | Unknown | 0 |
| 20 | UINT32 | Unknown | 0 |
| 24 | Byte | Gem1 | 13 |
| 25 | Byte | Gem2 | 13 |
| 26 | Byte | RebornEffect | 200 |
| 27 | Byte | Unknown | 0 |
| 28 | Byte | Plus | 9 |
| 29 | Byte | Bless | 7 |
| 30 | Byte | Enchant | 255 |
| 31 | Byte | Unknown | 0 |
| 32 | UINT32 | RestrainType | 0 |
| 36 | UINT32 | Unknown | 0 |
| 40 | UINT32 | Unknown | 0 |
