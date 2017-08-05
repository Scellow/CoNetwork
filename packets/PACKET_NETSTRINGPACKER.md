TQs NetStringPacker is essentially just a list of variable length strings.


| Offset | Data Type | Description | Example |
|---|---|---|---|
| 0 | BYTE | Strings Count | 2 |
| 1 | BYTE | String Length | 5 |
| 2 | STRING | String Content | Hello |
| 7 | BYTE | String Length | 3 |
| 8 | STRING | String Content | You |
