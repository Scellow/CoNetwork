**MsgAction:** This packet is used to control and verify many different types of actions between the game client and game server. It contains the ID of an entity performing the action, a type of action being performed and a variable amount of information, often with various fields being used.

It is worth noting that it is very common for each 'Data' field to be broken into 2 UINT16 accessors to set 'high' and 'low' values.

**Patch 5017:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 24 |
| 2 | UINT16 | Packet Identifier | 1010 |
| 4 | UINT32 | Client Timestamp | 123123 |
| 8 | UINT32 | Character ID | 1000001 |
| 12 | UINT32 | Data1 | 321 |
| 16 | UINT32 | Data2 | 123 |
| 20 | UINT16 | Direction | 1 |
| 22 | [[msgactiontype|ActionType]] | Action | 137 |

**Patch 5165:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 10010 |
| 8 | UINT32 | Character ID | 1000001 |
| 12 | UINT32 | Data1 | 321 |
| 16 | UINT32 | Client Timestamp | 123123 |
| 20 | [[msgactiontype|ActionType]] | Action | 137 |
| 22 | UINT16 | Direction | 1 |
| 24 | UINT32 | Data2 | 123 |
| 28 | UINT32 | Data3 | 123 |

**Patch 5212:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 42 |
| 2 | UINT16 | Packet Identifier | 10010 |
| 8 | UINT32 | Character ID | 1000001 |
| 12 | UINT32 | Data1 | 321 |
| 16 | UINT32 | Data2 | 321 |
| 20 | UINT32 | Client Timestamp | 123123 |
| 24 | [[msgactiontype|ActionType]] | Action | 137 |
| 26 | UINT16 | Direction | 1 |
| 30 | UINT32 | Data3 | 123 |
| 34 | UINT32 | Data4 | 123 |
| 38 | UINT32 | Data5 | 123 |

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 38 |
| 2 | UINT16 | Packet Identifier | 10010 |
| 4 | UINT32 | Character Identity | 1000000 |
| 8 | UINT32 | Action Data | 321 |
| 12 | UINT32 | Action Details | 321 |
| 16 | UINT32 | Client Timestamp | 123123 |
| 20 | [[msgactiontype|ActionType]] | Action Type | 137 |
| 22 | UINT16 | Direction | 0 |
| 24 | UINT16 | X | 400 |
| 26 | UINT16 | Y | 400 |
| 28 | UINT32 | Map | 1002 |
| 32 | UINT16 | Color | 0 |
| 36 | BOOL | Mounted Flag | 0 |
| 37 | BOOL | Action Response Flag | 0 |
