**MsgPigeon:** This packet is used to request and control player Broadcasts.  Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 + Strings.TotalLength |
| 2 | UINT16 | Packet Identifier | 2050 |
| 4 | [[msgbroadcastactiontype|BroadcastActionType]] | Action | BroadcastActionType.SendBroadcast |
| 8 | INT32 | MessageId | 0 |
| 12 | [[msgnetstringpacker|NerStringPacker]] | Strings  | 1 5 Hello |
