**MsgEudemonInfo:** This packet was implemented in the base implementation of their game and server, but was removed before Conquer Online 1.0 Alpha. It can be assumed that this packet was originally drafted for the Eudemons system in Eudemons Online. The packet was sent from the game server to the client to initialize the spawning of an Eudemon (similar to the [[MsgNpcInfoEx]] packet). 

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 38 + Name Length |
| 2 | UINT16 | Packet Identifier | 1116 |
| 4 | UINT32 | Identity | 500001 |
| 8 | UINT32 | Mesh | 501 |
| 12 | UINT64 | Status | 0 |
| 20 | UINT32 | Owner Identity | 1000000 |
| 24 | UINT16 | Maximum Health | 108 |
| 26 | UINT16 | Current Health | 108 |
| 28 | UINT16 | X Position | 250 |
| 30 | UINT16 | Y Position | 130 |
| 32 | BYTE | Direction | 0 |
| 33 | BYTE | Action | 0 |
| 34 | UINT32 | Monster Type | 0 |
| 38 | BYTE | Name Length | 0 |
| | CHAR[Name Length]| Name| |

Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
