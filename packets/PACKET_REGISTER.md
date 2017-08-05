**MsgRegister:** This packet is sent from the game client to the game server. It contains initial character information from the character creation screen, such as the name, body type, profession, and mac address. This information needs to be verified with the server to ensure that the name is not taken and contains valid characters, and that the body and profession are valid.

**Patch 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]], [[http://chained2pvp.com/profile/395-vander/|Vander]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 60 |
| 2 | UINT16 | Packet Identifier | 1001 |
| 4 | CHAR[16] | Account | Spirited |
| 20 | CHAR[16] | Name | Test |
| 36 | CHAR[16] | Password (yes, really) | test |
| 52 | UINT16 | Model | 1003 |
| 54 | UINT16 | Class | 10 |
| 56 | UINT32 | Identity | 1000000 |

**Patch 5165:** Contributed by [[http://chained2pvp.com/user/25-caparzo/|Caparzo]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 104 |
| 2 | UINT16 | Packet Identifier | 1001 |
| 20 | CHAR[16] | Character Name | TestPlayer |
| 52 | UINT16 | Character Body | 1003 |
| 54 | UINT16 | Character Class | 10 |
| 56 | UINT32 | Character Identity | 1000000 |
| 60 | UINT16[6] | Client MacAddress | 00,10,5A,44,12,B5 |

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 124 |
| 2 | UINT16 | Packet Identifier | 1001 |
| 4 | UINT32 | [[msgregistertype|Request Type]] | 0 |
| 8 | CHAR[16] | Account Name //(Unused)// | |
| 24 | CHAR[16] | Forename | Test |
| 40 | CHAR[16] | Surname //(Unused)// | |
| 56 | CHAR[16] | Password //(Unused)// | |
| 72 | UINT16 | Character Body | 1003 |
| 74 | UINT16 | Character Class | 10 |
| 76 | UINT32 | Character Identity | 1000000 |
| 80 | CHAR[12] | Client MacAddress | 0A0027000000 |
The rest of this packet is confirmed empty space (32 bytes).\\
All "unused" fields are now not implemented in the client.
