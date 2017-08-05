**MsgTradeBuddy:** This packet is used to send requests relating to the trade partner system and contains multiple TradePartnerAction types

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 2046|
| 4 | UINT32 | Id | 123123 |
| 8 | Byte | Action | 1|
| 9 | Bool | IsOnline| 1|
| 10 | UINT32 | HoursLeft | 0 |
| 14| UINT16 | Unknown | 0 |
| 16 | Byte[16] | Name| "Pro4Never       " |
