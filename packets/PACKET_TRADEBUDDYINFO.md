**MsgTradeBuddyInfo** This packet is used to list information regarding trade partners. For actions related to adding/removing trade partners, reference MsgTradeBuddy

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 34 |
| 2 | UINT16 | Packet Identifier | 2046|
| 4 | UINT32 | Id | 123123 |
| 8 | UINT32 | Lookface | 1 |
| 12 | Byte| Level | 130 |
| 13 | Byte| Profession| 15 |
| 14 | UINT16 | PKPoints| 0 |
| 16 | UINT32  | GuildID| 0 |
| 20 | UINT32  | GuildRank| 0 |
| 24 | UINT16 | Unknown | 0 |
| 26 | BYTE[16] | Name | “Pro4Never ” |
