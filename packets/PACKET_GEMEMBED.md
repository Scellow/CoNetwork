**MsgGemEmbed:** This packet is sent from the game client to the game server. It is used to add a gem to an empty socket, or remove a gem that is already embedded.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2071 |
| 4 | UINT32 | Sender Identity | 1000000 |
| 8 | UINT32 | Item Identity | 123 |
| 12 | UINT32 | Gem Identity | 321 |
| 16 | UINT16 | Location | 1 |
| 18 | UINT16 | Action | 0 or 1 |
