**MsgDH:** MsgDH defines TQ Digital Entertainment's transport wrapper for the DH key exchange and delivering the server's public key and initial DH parameter constants. This is the first step in the DH key exchange.

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | CHAR[11] | Header Pad | ... |
| 11 | UINT32 | Length | 352 |
| 15 | UINT32 | Random Pad Len | 42 |
| 19 | CHAR[42] | Random Pad | ... |
| 61 | UINT32 | Encryption IV Len | 8 |
| 65 | CHAR[8] | Encryption IV | ... |
| 73 | UINT32 | Decryption IV Len | 8 |
| 77 | CHAR[8] | Decryption IV | ... |
| 85 | UINT32 | Prime Modulo Len | 128 |
| 89 | CHAR[128] | Prime Modulo | ... |
| 217 | UINT32 | Generator Len | 2 |
| 221 | CHAR[2] | Generator | ... |
| 223 | UINT32 | Public Key Len | 128 |
| 227 | CHAR[128] | Public Key | ... |

**Notes:** The length offset value of the packet is 3 bytes less than the actual length. If the length offset is set to the actual length, the client will hang (expecting the remaining bytes). In addition, this packet requires the game server footer "TQServer".
