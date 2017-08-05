**MsgContribute:** This packet is sent between the client and game server. It contains reward information for the player's contribution to helping apprentice players.

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira|Felipe Vieira]].

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 40 |
| 2 | UINT16 | Packet Identifier | 2067 |
| 4 | UINT32 | Packet Type | 5 |
| 8 | UINT32 | User Identity | 1000000 |
| 24 | UINT64 | Prize Experience | 600 |
| 32 | UINT16 | Prize Heaven Blessing | 3 |
| 34 | UINT16 | Prize Composing | 200 |
**Notes:** 600 Experience is 1 ExpBall, Heaven Blessing is per hour and Composing 100 is 1. 
