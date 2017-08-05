**MsgConnect:** This packet is created by the client after it processes the [[MsgConnectEx]] packet, disconnecting from the account server, and connecting to the game server. It sends this packet to the game server to pass authenticated information from the account server. It also sends a second packet to the account server with the contents of [[resdat|Res.dat]].

**Security Warning**: The identity and additional data fields are passed from the account server; therefore, it is expected that the account server encrypts this information before sending it to the client. 

**Patch 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]\\

Account Server:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 |
| 2 | UINT16 | Packet Identifier | 1052 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | File Contents | 10 |
| 12| CHAR[16] | File Name | [[resdat|Res.dat]] |

Game Server:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 |
| 2 | UINT16 | Packet Identifier | 1052 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | Additional Data | 2 |
| 12 | CHAR[4] | Client Build Version | 117 |
| 16 | CHAR[12] | Language | English |

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]\\

Account Server:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 |
| 2 | UINT16 | Packet Identifier | 1052 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | File Contents | 10 |
| 12| CHAR[16] | File Name | [[resdat|Res.dat]] |

Game Server:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 |
| 2 | UINT16 | Packet Identifier | 1052 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | Additional Data | 2 |
| 12 | UINT16 | Client Build Version | 130 |
| 14 | CHAR[2] | Language | En |
| 16 | BYTE[6] | Mac Address | 0A, 0B, 0C, 0D, 0E, 0F |
| 24 | UINT32 | [[resdat|Res.dat]] Contents | 10 |
Notes: The client does not write to offsets 22 and 23. It is possible that if the mac address cannot be retrieved that the Mac Address field will be zero or spell "LOOP" in ASCII for "loopback adapter".
