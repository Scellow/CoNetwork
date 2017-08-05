**MsgTaskDialog:** This packet is used to interact with a NPC and contains multiple DialogAction types

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 + Strings.TotalLength |
| 2 | UINT16 | Packet Identifier | 2032 |
| 4 | UINT32 | Id | 123123 |
| 8 | UINT16 | Avatar | 10 |
| 10 | BYTE | OptionId | 0 |
| 11 | [[msgdialogaction|DialogActionType]] | Action | DialogActionType.Text |
| 12 | [[msgnetstringpacker|NetStringPacker]] | Strings | 1 5 Hello |
