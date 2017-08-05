**MsgLogin:** This internal packet is sent by TQ Digital Entertainment's NPC server to initialize synchronization between the NPC server and Game server. It is processed similarly to how accounts are processed using [[MsgAccount]] (even processed in the same method but with preprocessor conditions for disabling RC5). The server uses this packet to send the version of the NPC server to the game server, along with an account and password in plain text. 

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 40 |
| 2 | UINT16 | Packet Identifier | 1002 |
| 4 | UINT32 | Version | 100 |
| 8 | CHAR[16] | Account | (empty string) |
| 24 | CHAR[16] | Password | (empty string) |

Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
