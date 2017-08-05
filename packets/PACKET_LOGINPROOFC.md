**MsgLoginProofC:** This packet is sent during the client's authentication state from the account server. The keys in this packet are for the password cipher, representing the client's proof of K (the client key). It's sent to start the final challenge for verifying the player's inputted password.

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 262 |
| 2 | UINT16 | Packet Identifier | 1214 |
| 4 | BYTE | Length of the Response Session Key |  |
| 5 | BYTE[] | Response Session Key | |
| 133 | BYTE | Length of Proof of K |  |
| 134 | BYTE[] | Proof of K | |
