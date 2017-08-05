**MsgDataArray:** This packet is used to send a list of ItemIds to be used in systems such as composition or breeding.

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 24 |
| 2 | UINT16 | Packet Identifier | 2036 |
| 4 | DataArrayActionType | Action | DataArrayActionType.Compose |
| 5 | INT32[] | Items | 2 111 112  |
