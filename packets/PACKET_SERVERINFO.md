**MsgServerInfo:** This packet is sent between the game server and client to set client-side rules in regards to "Conquer Online 2.0" gameplay vs. "Conquer Online Classic" gameplay. The packet was first introduced with the classic servers to instruct the client on when and if to show the shopping mall and how player potency was calculated.

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 |
| 2 | UINT16 | Packet Identifier | 2079 |
| 4 | UINT32 | Server Type | 0 |
| 8 | UINT32 | Potency Type | 0 |

**Notice: **For the server and potency types above, \\
0 = Standard Conquer Online 2.0 Server\\
1 = Classic Conquer Online 2.0 Server\\
