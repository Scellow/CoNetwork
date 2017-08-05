**MsgUserInfo:** This packet is sent from the game server to the game client. It contains character information from the game database, such as the name, body type, profession, and character attributes. In response to this packet, the client will send a character location request. Check the [[msgaction|MsgAction]] packet for details.

**Patch 4330:** Contributed by [[http://chained2pvp.com/profile/8-spirited|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (61 + String List) | 83 |
| 2 | UINT16 | Packet Identifier | 1006 |
| 4 | UINT32 | Identity | 1000000 |
| 8 | UINT32 | [[MeshFormula|Mesh]] | 1003 |
| 12 | UINT16 | Hairstyle | 535 |
| 16 | UINT32 | Silver | 10000 |
| 20 | UINT64 | Experience | 0 |
| 40 | UINT16 | Strength | 7 |
| 42 | UINT16 | Agility | 2 |
| 44 | UINT16 | Vitality | 4 |
| 46 | UINT16 | Spirit | 0 |
| 48 | UINT16 | Attributes | 0 |
| 50 | UINT16 | Health | 123 |
| 52 | UINT16 | Mana | 0 |
| 54 | UNIT16 | PkPoints | 0 |
| 56 | BYTE | Level | 1 |
| 57 | BYTE | Class | 10 |
| 58 | BOOL | Autoallot | 1 |
| 59 | BYTE | Rebirths | 0 |
| 60 | BOOL | ShowName | 1 |
| 61 | BYTE | String List Count | 2 |
|  | BYTE | Character Name Length | 13 |
|  | CHAR[] | Character Name | CptMotorcycle |
|  | BYTE | Spouse Name length | 4 |
|  | CHAR[] | Spouse | None |

**Patch 5165:** Contributed by [[http://chained2pvp.com/user/25-caparzo/|Caparzo]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (87 + String List) | 110 |
| 2 | UINT16 | Packet Identifier | 1006 |
| 4 | UINT32 | Character Identity | 1000000 |
| 8 | UINT32 | Mesh | 501003 |
| 12 | UINT16 | Hair Style | 418 |
| 14 | UINT32 | Silver | 10000 |
| 18 | UINT32 | Conquer Points | 10000 |
| 22 | UINT64 | Experience | 0 |
| 50 | UINT16 | Strength | 4 |
| 52 | UINT16 | Agility | 6 |
| 54 | UINT16 | Vitality | 12 |
| 56 | UINT16 | Spirit | 0 |
| 58 | UINT16 | Attribute Points | 0 |
| 60 | UINT16 | Health Points | 12 |
| 62 | UINT16 | Spirit Points | 0 |
| 64 | UINT16 | Player Kill Points | 0 |
| 66 | BYTE | Level | 1 |
| 67 | BYTE | Class | 10 |
| 69 | BYTE | Reborn Count | 0 |
| 71 | UINT32 | Quiz Points | 0 |
| 87 | BYTE | String List Count | 2 |
|  | BYTE | Character Name Length | 10 |
|  | CHAR[] | Character Name | PlayerTest |
|  | BYTE | Wife Name length | 10 |
|  | CHAR[] | Wife Name | PlayerWife |
 
**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (122 + String List) | 130 |
| 2 | UINT16 | Packet Identifier | 1006 |
| 4 | UINT32 | Character Identity | 1000000 |
| 8 | UINT16 | Appearance | 3 |
| 10 | UINT32 | Mesh | 501003 |
| 14 | UINT16 | Hair Style | 418 |
| 16 | UINT32 | Silver | 10000 |
| 20 | UINT32 | Conquer Points | 10000 |
| 24 | UINT64 | Experience | 0 |
| 44 | UINT64 | Virtue | 0 |
| 52 | UINT16 | Strength | 4 |
| 54 | UINT16 | Agility | 6 |
| 56 | UINT16 | Vitality | 12 |
| 58 | UINT16 | Spirit | 0 |
| 60 | UINT16 | Attribute Points | 0 |
| 62 | UINT16 | Health Points | 12 |
| 64 | UINT16 | Spirit Points | 0 |
| 66 | UINT16 | PK Points | 0 |
| 68 | BYTE | Level | 1 |
| 69 | BYTE | Current Class | 10 |
| 70 | BYTE | Ancestor Class (2nd rb) | 10 |
| 71 | BYTE | Previous Class (2nd rb, else offset 70) | 10 |
| 73 | BYTE | Reborn Count | 2 |
| 77 | UINT16 | Coach Chance Value P | 0 |
| 83 | UINT16 | Coach Day Info | 0 |
| 85 | UINT32 | VIP Level | 0 |
| 91 | UINT16 | TitleId | 0 |
| 93 | UINT32 | Bound Conquer Points | 10000 |
| 97 | BYTE | Subclass Id | 0 |
| 98 | UINT64 | Subclass Step-Level | 0 |
| 106 | UINT32 | Ride Points | 0 |
| 110 | BYTE | String List Count | 2 |
| 111 | BYTE | Character Name Length | 4 |
|  | CHAR[] | Character Name | Test |
|  | BYTE | Spouse Name length | 10 |
|  | CHAR[] | Spouse Name | None |
