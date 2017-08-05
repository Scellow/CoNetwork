**MsgItem:** MsgItem is sent from the game client to the game server. Item actions, market interface actions, and some interface updates are handled through this packet. Ping response is handled through this packet.

**Patch 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 20 |
| 2 | UINT16 | Packet Identifier | 1009 |
| 4 | UINT32 | Identity | 1000001 |
| 8 | UINT32 | Argument| 0 |
| 12 | UINT32 | [[MsgItemAction|Action]] | 27 |
| 16 | UINT32 | Timestamp | 42351641 |
