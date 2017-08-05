**MsgTick:** This packet is sent from the game server to the client, and then back again from the client to the game server in a round-trip for checking network congestion. The packet is responsible for the "Warning: the network is congested" message that appears in the top-left of the client screen. It's secondary purpose is for verifying that the user is not a bot (Conquer 1.0 and early Conquer 2.0).

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | S->C Example | C->S Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 ||
| 2 | UINT16 | Packet Identifier | 1012 ||
| 4 | UINT32 | Character Identity | 1000000 ||
| 8 | UINT32 | Timestamp | 0 | 1807831 |
| 12 | BYTE[16] | Random Padding | random() ||
| 28 | UINT32 | Character Name (2 Bytes) | 0 | 56925 |

Notes: The timestamp field requires to be XORed by the Character Identity field before server processing of this packet. The character name (the first two bytes of the character name) has a similar requirement: XORed by 0x9823.
