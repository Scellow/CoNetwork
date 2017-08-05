**MsgPCNum:** This packet is sent during the client's authentication state. It's sent to the account server after the [[MsgConnectEx]] packet has been processed by the client. The packet contains the player's mac address for successful login recording.

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 52 |
| 2 | UINT16 | Packet Identifier | 1100 |
| 4 | UINT32 | Account Identity | 1000000 |
| 8 | CHAR[40] | Mac Address | 0A0B0C0D0E0F |
Notes: Client forces null terminator at offset 48 (byte). No other information is written to the packet past offset 48. If the mac address could not be retrieved, the mac address field will not be assigned. 
