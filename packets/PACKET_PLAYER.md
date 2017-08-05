**MsgPlayer:** This packet is sent to the observing clients on the map server when the actor enters their screen or an acting client observes the character as they enter its screen. The packet contains the player's character spawn information.

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira/|Felipe Vieira]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 100 + CharacterName + CharacterMate |
| 2 | UINT16 | Packet Identifier | 10014 |
| 4 | UINT32 | [[meshformula|Mesh]] | 1003 |
| 8 | UINT32 | User Identity | 1000000 |
| 12 | UINT16 | Syndicate Identity | 30 |
| 15 | BYTE | Syndicate Rank | 100 |
| 16 | UINT64 | Flags | 8 |
| 24 | UINT32 | Helmet | 118109 |
| 28 | UINT32 | Garment | 0 |
| 32 | UINT32 | Armor | 130109 |
| 40 | UINT32 | Left Hand | 410339 |
| 44 | UINT32 | Right Hand | 480339 |
| 48 | UINT16 | Life | 15000 |
| 52 | UINT32 | Hair Style | 316 |
| 54 | UINT16 | Map X | 430 |
| 56 | UINT16 | Map Y | 378 |
| 58 | BYTE | Direction | 7 |
| 59 | BYTE | Entity Action | 0 |
| 61 | BYTE | Reborn | 2 |
| 62 | BYTE | Level | 130 |
| 66 | BYTE | Window Spawn | 1 |
| 70 | UINT16 | Shared Battle Power | 13 |
| 77 | UINT32 | Flower Charm | 0 |
| 81 | BYTE | Nobility Rank | 12 |
| 85 | UINT16 | Armor Color | 3 |
| 87 | UINT16 | Shield Color | 4 |
| 89 | UINT16 | Helmet Color | 3 |
| 91 | UINT32 | Quiz Points | 6546 |
| 95 | [[msgnetstringpacker|NetStringPacket]] | Strings | 2 4 Name 6 Spouse |

**Note:** Not sure if the client or something being sent wrongly, but it bugs the screen when wearing a shield jumping like a ninja.
