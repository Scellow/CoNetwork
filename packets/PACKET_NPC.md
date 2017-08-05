**MsgNpc:** This packet is used to interact with a NPC and contains multiple DialogAction types

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 16 |
| 2 | UINT16 | Packet Identifier | 2031 |
| 4 | UINT32 | Id | 123123 |
| 8 | UINT32 | Data | 10 |
| 12 | [[msgnpcaction|NpcActionType]] | Action | NpcAction.Activate |
| 14 | UINT16 | Sort | 0 |
