**MsgEncryptCode:** This packet is sent during the client's on-connect state with the Account Server. It's sent to the client from the Account Server to begin the packet exchange process. This random number acts as a seed for Rivest Cipher 5 in the client, used for encrypting the password to be sent over the network. This cipher was eventually replaced; however, this packet is still sent to start the packet exchange process.

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 8 |
| 2 | UINT16 | Packet Identifier | 1059 |
| 4 | UINT32 | Seed | 10000 |
