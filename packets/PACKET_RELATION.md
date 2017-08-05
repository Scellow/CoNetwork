**MsgRelation:** This packet is sent from the game server to the game client in newer client versions when sending requests. It is used to display relation data as well as battle power and level to verify a target's identity.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Sender Identity | 1000000 |
| 8 | UINT32 | Target Identity | 1000001 |
| 12 | UINT32 | Level | 130 |
| 16 | UINT32 | BattlePower | 155 |
| 20 | UINT32 | IsSpouse | 0 |
| 24 | UINT32 | IsApprentice | 0 |
| 28 | UINT32 | IsTradePartner | 0 |
