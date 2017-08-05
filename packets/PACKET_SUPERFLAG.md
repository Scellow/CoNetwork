**MsgSuperFlag:** This packet is used to record and teleport to previous locations using the MemoryAgate

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 + Count * 48 + 8 |
| 2 | UINT16 | Packet Identifier | 2110|
| 4 | UINT32 | Action | 1 |
| 8 | UINT32 | ItemId | 100 |
| 12 | UINT32 | Unknown12 | 0 |
| 16 | UINT32 | Unknown16 | 0|
| 20 | UINT32 | Unknown20 | 0|
| 24 | UINT32 | Durability | 20|
| 28 | UINT32 | Locations Count | 1 |
| 32 | AgateLocation[] | Locations | 1 1002 440 400 etc|


Each Location consists of 48 bytes of data in the following format

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT32 | Id | 1 |
| 4 | UINT32 | Map | 1002 |
| 8 | UINT32 | X | 440 |
| 12 | UINT32 | Y | 400 |
| 16 | UINT32 | Unknown| 0 |
| 20 | UINT32 | Unknown | 0 |
| 24 | UINT32 | Unknown | 0 |
| 28 | UINT32 | Unknown | 0 |
| 32 | UINT32 | Unknown | 0 |
| 36 | UINT32 | Unknown | 0 |
| 40 | UINT32 | Unknown | 0 |
| 44 | UINT32 | Unknown | 0 |
| 48 | UINT32 | Unknown | 0 |
