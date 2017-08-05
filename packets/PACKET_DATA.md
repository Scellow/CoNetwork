**MsgData:** This packet is sent between the game server and client to exchange interval based data, such as variable rates (vigor or anti-cheat parameters) or the server's date and time. The packet updates rates of interval values after being processed by the client. The client can also request the time and other variable rates from the server.

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 36 |
| 2 | UINT16 | Packet Identifier | 1033 |
| 4 | UINT32 | [[msgdatatype|Update Type]] | 0 |
| 8 | UINT32 | Year - 1900 (or data) | 115 |
| 12 | UINT32 | Month - 1 | 9 |
| 16 | UINT32 | Day of Year | 297 |
| 20 | UINT32 | Day | 24 |
| 24 | UINT32 | Hour | 23 |
| 28 | UINT32 | Minute | 55 |
| 32 | UINT32 | Second | 0 |
