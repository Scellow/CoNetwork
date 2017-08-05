**MsgEudemonAttrib:** This packet was implemented in the base implementation of their game and server, but was removed before Conquer Online 1.0 Alpha. It can be assumed that this packet was originally drafted for the Eudemons system in Eudemons Online. The packet was sent from the game server to the client to add attribute effects to an Eudemon (similar to the [[MsgUserAttrib]] packet for players). 

** Packet Definition: ** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]].

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 |
| 2 | UINT16 | Packet Identifier | 2037 |
| 4 | UINT32 | Identity | 500001 |
| 8 | UINT32 | Attribute Count | 1 |
| 12 | ATTRIB_INFO[] | Attribute Info |  |

** ATTRIB_INFO Definition: ** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]].

| Data Type | Description | Example |
|---|---|---|---|
| UINT32 | [[MsgEudemonAttribType|Attribute Type]] | 4 |
| UINT32 | Attribute Data | 12 |
