**MsgTitle:** This packet is used to list or change a player's title.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 20+TitleCount|
| 2 | UINT16 | Packet Identifier | 1130 |
| 4 | UINT32 | TitleType | 11|
| 8 | UINT32 | Action | 3 |
| 12 | Byte | TitleCount | 1 |
| 13 | TitleType[] | Titles | 11 |
