**MsgConnectEx:** This packet is sent during the client's authentication state to either accept or reject the client's attempt to login to the selected game server. The length of an acceptation packet
is 52 (because it includes the authentication code, port, and IP address). The length of a rejection, 12. The authentication code and identity are XORed by 0x4321 in the original client; however, this method of "protection" will not suffice. The game server IP address cannot be a localhost address (127.x.x.x). Local network and public network addresses are accepted.

**Patches 4274 - 4330:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]\\
Acceptance Example:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 32 |
| 2 | UINT16 | Packet Identifier | 1055 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | Authentication Code | 2 |
| 12 | CHAR[16] | Game Server IP Address | 192.168.1.2 |
| 28 | UINT32 | Game Server Port | 5816 |

Rejection Example:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 28 |
| 2 | UINT16 | Packet Identifier | 1055 |
| 8 | UINT32 | [[rejectionenum|Rejection Code]] | 1 |
| 12 | CHAR[16] | Message (GB2312 Encoding) | 帐号名或口令错 |
**Notes:** The following messages are some I found by reversing the client.\\
"Invalid account name or password." (1): 帐号名或口令错\\
"The server is down!" (10): 服务器未启动\\
"Please re-login later." (11): 请稍后重新登录\\
"This account is banned." (12): 该帐号被封号\\
"Unknown Error" (999): 数据库错误\\

<code>
var MSGCONNECTEX_INVALID_ACCOUNT = []byte { // 帐号名或口令错 (1)
	0xD5, 0xca, 0xba, 0xc5, 0xc3, 0xfb, 0xbb, 0xf2,
	0xbf, 0xda, 0xc1, 0xee, 0xb4, 0xed, 0x00, 0x00 }
var MSGCONNECTEX_SERVER_DOWN = []byte { // 服务器未启动 (10)
	0xb7, 0xfe, 0xce, 0xf1, 0xc6, 0xf7, 0xce, 0xb4, 
	0xc6, 0xf4, 0xb6, 0xaf }
var MSGCONNECTEX_LOGIN_LATER = []byte { // 请稍后重新登录 (11)
	0xc7, 0xeb, 0xc9, 0xd4, 0xba, 0xf3, 0xd6, 0xd8, 
	0xd0, 0xc2, 0xb5, 0xc7, 0xc2, 0xbc, 0x00, 0x00 }
var MSGCONNECTEX_BANNED_ACCOUNT = []byte { // 该帐号被封号 (12)
	0xb8, 0xc3, 0xd5, 0xca, 0xba, 0xc5, 0xb1, 0xbb,
	0xb7, 0xe2, 0xba, 0xc5, 0x00, 0x00, 0x00, 0x00 }
</code>

**Patch 5635:** Contributed by [[http://chained2pvp.com/user/8-spirited/|Spirited]]\\
Acceptance Example:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 52 |
| 2 | UINT16 | Packet Identifier | 1055 |
| 4 | UINT32 | Client Identity | 1000000 |
| 8 | UINT32 | Authentication Code | 2 |
| 12 | UINT32 | Game Server Port | 5816 |
| 20 | CHAR[32] | Game Server IP Address | 192.168.1.2 |

Rejection Example:
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 12 |
| 2 | UINT16 | Packet Identifier | 1055 |
| 8 | UINT32 | [[rejectionenum|Rejection Code]] | 10 |
