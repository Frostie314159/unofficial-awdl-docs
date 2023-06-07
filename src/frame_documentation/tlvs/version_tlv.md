# Version TLV

A version tlv consists of two parts, the version, which is in the normal [format](../version.md), and the device class.

## Structure

| Byte | Meaning      | Value Type                    |
| ---- | ------------ | ----------------------------- |
| 0x00 | Version      | [AWDL Version](../version.md) |
| 0x01 | Device Class | =                             |

## Device Class

In the TLV the type of the transmitting device is encoded as a one byte value, as mentioned above.

| Value | Device Type    |
| ----- | -------------- |
| 0x01  | MacOS          |
| 0x02  | iOS or WatchOS |
| 0x08  | tvOS           |


