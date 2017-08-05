**MsgNationality:** This packet is sent to the game client to update the player's country flag. The country flag appears near players' names after patch 5639. Strings must match a preset from a dictionary of countries names, found in Nationality.ini.

**Patch 6150:** Contributed by [[http://chained2pvp.com/profile/12-sedat/|Sedat]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 10 |
| 2 | UINT16 | Packet Identifier | 2430 |
| 4 | UINT32 | Player ID | 11111111111 |
| 8 | Byte | [[MsgNationalityID|Country ID]] | 10 |
