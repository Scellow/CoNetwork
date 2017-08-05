**MsgNpcInfo:** This packet is used to spawn NPCs to players.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2030|
| 4 | UINT32 | UniqueID | 123123 |
| 8 | UINT32 | StaticID | 123123 |
| 12 | UINT16 | X | 100 |
| 14 | UINT16 | Y | 100 |
| 16 | UINT16 | Lookface | 100 |
| 18 | UINT16 | NpcType | 2 |
| 20 | UINT16 | RoleType | 2 |
| 22 | String[] | Names | 0 |
