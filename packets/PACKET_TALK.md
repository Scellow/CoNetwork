**MsgTalk:** This packet is sent between the game client and server to exchange messages. The messages are used to control the client during login to the game server, and to socialize with other players on the server. The packet includes player meshes in patches 5017 and higher for private whisper windows. Suffix is used for offline messages, and usually contains the date in the format yyyyMMdd.

**Patch 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (20 + Len(Sender, Recipient, Suffix, Message)) | 43 |
| 2 | UINT16 | Packet Type | 1004 |
| 4 | UINT32 | Color in ARGB | 00FF0000 |
| 8 | UINT16 | [[chattoneenum|Tone]] | 2101 |
| 10 | UINT16 | [[chatstyleenum|Style]] | 0 |
| 12 | UINT32 | Identity | 1000000 |
| 16 | BYTE | String List Count | 4 |
|  | BYTE | Sender's Name Length | 6 |
|  | CHAR[] | Sender's Name | SYSTEM |
|  | BYTE | Recipient's Name Length | 8 |
|  | CHAR[] | Recipient's Name | ALLUSERS |
|  | BYTE | Suffix Length | 0 |
|  | CHAR[] | Suffix | |
|  | BYTE | Message Length | 8 |
|  | CHAR[] | Message | NEW_ROLE |

**Patch 5165:** Contributed by [[http://chained2pvp.com/user/25-caparzo/|Caparzo]], [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (28 + Length from Sender's Name, Recipient's Name, Suffix, and Message) | 61 |
| 2 | UINT16 | Packet Type | 1004 |
| 4 | UINT32 | Text Color in ARGB | 00FF0000 |
| 8 | UINT16 | [[chattoneenum|Message Tone]] | 2000 |
| 10 | UINT16 | [[chatstyleenum|Message Style Flag]] | 0 |
| 12 | UINT32 | Sender's Identity | 1000000 |
| 16 | UINT32 | Recipient's [[meshformula|Mesh]] | 501002 |
| 20 | UINT32 | Sender's [[meshformula|Mesh]] | 501002 |
| 24 | BYTE | String List Count | 4 |
|  | BYTE | Sender's Name Length | 7 |
|  | CHAR[] | Sender's Name | Player1 |
|  | BYTE | Recipient's Name Length | 7 |
|  | CHAR[] | Recipient's Name | Player2 |
|  | BYTE | Suffix Length | 8 |
|  | CHAR[] | Suffix | 20140518 |
|  | BYTE | Message Length | 11 |
|  | CHAR[] | Message | Hello world |

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length (31 + Length from Sender's Name, Recipient's Name, Suffix, and Message) | 63 |
| 2 | UINT16 | Packet Type | 1004 |
| 4 | UINT32 | Text Color in ARGB | 0xFFFFFF00 |
| 8 | UINT16 | [[chattoneenum|Message Tone]] | 2000 |
| 10 | UINT16 | [[chatstyleenum|Message Style Flag]] | 0 |
| 12 | UINT32 | Sender's Identity / Time | (hour * 100) + min |
| 16 | UINT32 | Recipient's [[meshformula|Mesh]] | 501002 |
| 20 | UINT32 | Sender's [[meshformula|Mesh]] | 501002 |
| 24 | BYTE | String List Count | 6 |
|  | BYTE | Sender's Name Length | 7 |
|  | CHAR[] | Sender's Name | Player1 |
|  | BYTE | Recipient's Name Length | 7 |
|  | CHAR[] | Recipient's Name | Player2 |
|  | BYTE | Suffix Length | 8 |
|  | CHAR[] | Suffix | 20140518 |
|  | BYTE | Message Length | 11 |
|  | CHAR[] | Message | Hello world |
|  | BYTE | Unreferenced String Length (empty string used in client) | 0 |
|  | BYTE | Unreferenced String Length (empty string used in client) | 0 |
