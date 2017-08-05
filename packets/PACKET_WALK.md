**MsgWalk:** This packet is used to control ground movement of the player. In recent versions there are many different subtypes used rather than the classic Walk-Run types.

**Patch 5017:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 10 |
| 2 | UINT16 | Packet Identifier | 1005 |
| 4 | UINT32 | Character ID | 1000001 |
| 8 | BYTE | [[directions|Direction]] | 1 |
| 9 | BYTE | [[msgmovementtype|Movement Type]] | MovementType.Walk |

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]] and [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 24 |
| 2 | UINT16 | Packet Identifier | 10005 |
| 4 | UINT32 | [[directions|Direction]] | 1 |
| 8 | UINT32 | Character ID | 1000001 |
| 12 | UINT32 | [[msgmovementtype|Movement Type]] | MovementType.Walk |
| 16 | UINT32 | Timestamp | 123123 |
| 20 | UINT32 | Map ID | 1002 |

**Patch 6132:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 24 |
| 2 | UINT16 | Packet Identifier | 10005 |
| [[googleprotocolbuffers|Google Protocol Buffer]] (Offsets 4 - 20) ||||
| 4 | UINT32 | [[directions|Direction]] | 1 |
| 8 | UINT32 | Character ID | 1000001 |
| 12 | UINT32 | [[msgmovementtype|Movement Type]] | MovementType.Walk |
| 16 | UINT32 | Timestamp | 123123 |
| 20 | UINT32 | Map ID | 1002 |
