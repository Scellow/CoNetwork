**MsgName:** This packet is a variable length packet sent between the client and game server to request, set and modify certain strings (such as spouse name). It can also be used to display client assets in game (effects, sounds, etc)


**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 13 + totalStringLength |
| 2 | UINT16 | Packet Identifier | 1015|
| 4 | UINT32 | Data | 1000001 |
| 8 | [[msgstringtype|StringType]]| Action | StringType.Mate |
| 9 | [[msgnetstringpacker|NetStringPacker]]| Strings | 1 5 Booty |
