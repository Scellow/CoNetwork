**MsgMagicInfo:** This packet is sent from the game server to the game client to add a spell or set its level.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Experience | 100 |
| 8 | UINT16 | Spell Type | 1000 |
| 10 | UINT16 | Level | 1 |
