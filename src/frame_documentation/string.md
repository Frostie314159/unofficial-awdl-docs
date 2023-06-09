# AWDL Strings

Sometimes you just have to transmit a string of characters within the AWDL protocol. For such purposes AWDL follows a certain format. Each strings is preceded by one byte, which is the length of the string plus one.

## Structure

| Byte                 | Meaning                                 | Value Type   |
| -------------------- | --------------------------------------- | ------------ |
| 0x00                 | Length of the following string plus one | 8bit Integer |
| 0x01-(0x01+length-1) | The string.                             | UTF-8 String |
