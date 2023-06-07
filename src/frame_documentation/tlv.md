# TLVs

AWDL uses normal TLVs, which consist of a one byte long type value, two bytes of length, followed by a dynamic amount of data.

| Byte(s)              | Meaning | Value Type    |
| -------------------- | ------- | ------------- |
| 0x00                 | Type    | 8bit Integer  |
| 0x01-0x02            | Length  | 16bit Integer |
| 0x03-(0x03 + Length) | Data    | --            |

## Types

Within the AWDL protocol exist 12 different types of TLVs, which are currently in use.

| Value | Type                       |
| ----- | -------------------------- |
| 0x02  | Service Response           |
| 0x04  | Synchronization Parameters |
| 0x05  | Election Parameters        |
| 0x06  | Service Parameters         |
| 0x07  | EHT Capabilities           |
| 0x0C  | Data Path State            |
| 0x10  | Arpa                       |
| 0x11  | IEEE 802.11 Container      |
| 0x12  | Channel Sequence           |
| 0x14  | Synchronization Tree       |
| 0x15  | Version                    |
| 0x20  | Election Parameters V2     |
| 0x24  | Unknown                    |
