**MsgWeather:** This packet is sent from the game server to the client for invoking weather on a map. This packet must be sent when the player changes maps; otherwise, the weather will be cleared by the client. 

**Patch 5615:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]

| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 20 |
| 2 | UINT16 | Packet Identifier | 1016 |
| 4 | UINT32 | [[msgweathertype|Weather Type]] | 2 |
| 8 | UINT32 | Intensity (Range: 0 - 999) | 50 |
| 12 | UINT32 | Direction (Range: 0 - 359) | 14 |
| 16 | UINT32 | Color in ARGB (Default: 0x00FFFFFF) | 0xFFFFFF00 |
Notes: This example produces a light rain shower.
