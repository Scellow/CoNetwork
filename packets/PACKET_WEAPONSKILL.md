**MsgWeaponSkill:** This packet is sent from the game server to the game client to set a character's proficiency with a specific weapon type.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Weapon Type | 480 |
| 8 | UINT32 | Level | 19 |
| 12 | UINT32 | Experience | 10000 |
| 16 | UINT32 | Experience Required | 2100000000 |
