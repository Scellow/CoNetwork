**MsgDice:** This packet is sent between the game server to the game client and is used to control actions and display results in the DiceKing mini game.

**Patch 5017:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 + Amount * 8 |
| 2 | UINT16 | Packet Identifier | 1113 |
| 4 | BYTE | [[msgdiceaction|DiceActionType]] | DiceActionType.ChipIn |
| 5 | BYTE | Amount | 1 |
| 6 | UINT16 | Unknown | 0 |
| 8 | UINT32 | DiceNpc Id | 1005 |
| 12 | UINT32 | DiceType | 1 |
| 16 | UINT32 | DiceData | 10000 |
