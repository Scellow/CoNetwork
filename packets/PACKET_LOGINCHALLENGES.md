**MsgLoginChallengeS:** This packet is sent during the client's authentication state from the account server. The keys in this packet are from the password cipher, representing the salt and public ephemeral value. It's sent as a request for the password challenge response packet.

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 653 |
| 2 | UINT16 | Packet Identifier | 1213 |
| 4 | BYTE | Length of the Public Ephemeral |  |
| 5 | BYTE[] | Public Ephemeral | |
| 391 | BYTE | Length of the Salt |  |
| 392 | BYTE[] | Salt | |
