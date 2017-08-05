**MsgNameChange:** This packet is used to handle the name change interface which TQ added in newer versions of conquer (around patch 5400)

**Patch 5517:** Contributed by [[http://chained2pvp.com/user/255-pro4never/|Pro4Never]]
| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | UINT16 | Packet Length | 26 |
| 2 | UINT16 | Packet Identifier | 2080 |
| 4 | NameChangeType | [[msgnamechangetype|NameChangeType]] | NameChangeType.Request |
| 6 | UINT16 | EditsCount | 1 |
| 8 | UINT16 | EditsAllowed | 1 |
| 10 | STRING(16) | Name | Pro4Never |
