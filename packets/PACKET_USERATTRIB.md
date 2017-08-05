**MsgUserAttrib:** Updates the client screen with new status and data and also some character data to players on the screen.

**Patch 5103:** Contributed by [[http://chained2pvp.com/profile/208-felipevieira/|Felipe Vieira]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 40 |
| 2 | UINT16 | Packet Identifier | 10017 |
| 4 | UINT32 | Identity | 1000002 |
| 8 | UINT32 | Update Count | 1000000 |
| 12 | UINT32 | [[MsgUserAttribType|Update Type]] | 1 |
| 16 | UINT64 | Value | 13500 |

**Note:** On some types you can send two UINT32 instead of one UINT64.
