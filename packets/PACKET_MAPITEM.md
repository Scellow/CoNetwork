**MsgMapitem:** This packet is sent from the game server to the game client to inform it of an item being added/removed from the map floor. it is also sent from the game client to the game server to request that an item be picked up.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Item Identity | 123 |
| 8 | UINT32 | Item Type | 500329 |
| 12 | UINT16 | X | 400 |
| 14 | UINT16 | Y | 400 |
| 16 | UINT16 | Color | 5 |
| 18 | UINT16 | Action | [[msggrounditemtype|GroundItemAction]].Pick |
