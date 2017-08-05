**MsgLoginAccountEx:** This packet was implemented in the base implementation of their game and server, but was removed before Conquer Online 1.0 Alpha. It can be assumed that this packet was originally drafted as an alternative to [[MsgConnect]] for 91 Game Portal logins. The packet was sent from the client to the game server (containing a mixture of the [[MsgAccount]] packet's content and [[MsgConnect]] packet's content). 

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 136 |
| 2 | UINT16 | Packet Identifier | 1090 |
| 4 | UINT32 | Login Type | 5 |
| 8 | CHAR[32] | Account | Spirited |
| 40 | CHAR[32] | Password | test |
| 72 | CHAR[32] | Server | Meteor |
| 104 | CHAR[32] | Info (Res.ini) | 0001 |

Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
