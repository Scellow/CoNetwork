**MsgCrossSwitch:** After sending this the server receives op 1015:60, reply with 1015:61. Switch guids can be below 4 billion but won't be correct.

**Patch 5635:** Contributed by [[http://chained2pvp.com/profile/151-mentalis/|Mentalis]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | |
| 2 | UINT16 | Packet Identifier | 2501 |
| 4 | UINT32 | Switch | 0 = normal, 1 = switch |
| 8 | UINT32 | Original Character Id | 1000001 |
| 12 | UINT32 | Switch Character Id | 1000002 |
| 16 | UINT16 | Item Count | 1 |
| 18 | Foreach Item |||
| | UINT32 | Original Item Id | 400 |
| | UINT32 | Switch Item Id | 450 |

**Notes:** sending this the server receives op 1015:60, reply with 1015:61.
Switch guids can be below 4 billion but won't be correct.
