**MsgFriend:** This packet is sent from the game client to the game server and vise versa to process friend actions. It allows the server to process friend requests, acceptances, and deletions, and allows the client to display friends and enemies in the friends/enemies window. The "Level" parameter in this packet was replaced by the use of the [[MsgFriendInfo]] packet. Facebook incorporation in some (if not all) clients relies on a now broken implementation, and will not function correctly.

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 68 |
| 2 | UINT16 | Packet Identifier | 1019 |
| 4 | UINT32 | Character Identity | 1000000 |
| 8 | BYTE | [[msgfriendactiontype|Action Type]] | 15 |
| 9 | BYTE | Online | 1 |
| 10 | UINT16 | Level ([[MsgFriendInfo|Unreferenced]]) | 0 |
| 12 | UINT32 | [[nobilityranktype|Nobility Rank]] | 3 |
| 16 | UINT32 | Gender | 1 |
| 20 | CHAR[16] | Forename | Test |
| 36 | CHAR[31] | Facebook ID | 123456789012345 |
| 67 | BYTE | Null Terminator (client forced) | 0 |
