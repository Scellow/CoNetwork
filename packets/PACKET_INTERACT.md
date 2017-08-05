**MsgInteract:** This packet is used to request and confirm many types of interactions such as attacking, casting spells or even proposing. It is worth noting that InteractType.Magic is hashed using the character ID/Timestamp values.

**Patch 5017:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 30 |
| 2 | UINT16 | Packet Identifier | 1022 |
| 4 | UINT32 | Timestamp | 123123 |
| 8 | UINT32 | SenderId | 1000001 |
| 12 | UINT32 | TargetId | 1000002 |
| 16 | UINT16 | X | 400 |
| 18 | UINT16 | Y | 450 |
| 20 | [[msginteracttype|InteractType]] | Action | InteractType.Shoot |
| 22 | UINT32 | Effect | 1 |
| 26 | UINT32 | ReturnedEffect | 0 |

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 38 |
| 2 | UINT16 | Packet Identifier | 1022 |
| 4 | UINT32 | Timestamp | 123123 |
| 8 | UINT32 | SenderId | 1000001 |
| 12 | UINT32 | TargetId | 1000002 |
| 16 | UINT16 | X | 400 |
| 18 | UINT16 | Y | 450 |
| 20 | [[msginteracttype|InteractType]] | Action | InteractType.Shoot |
| 22 | UINT32 | Effect | 1 |
| 26 | UINT32 | ReturnedEffect | 0 |
| 30 | [[msgActivationFlag|ActivationFlag]] | Activation | Activation.CriticalStrike |
| 34 | UINT32 | ActivationEffect | 0 |
