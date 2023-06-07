# Action Frames

AWDL action frames consist of a static 12byte header and a variable length body.

## Header

| Byte(s)   | Meaning                  | Default Value | Value Type    | Notes                                                   |
| --------- | ------------------------ | ------------- | ------------- | ------------------------------------------------------- |
| 0x00      | AF Type                  | 0x08          | byte          | --                                                      |
| 0x01      | [Version](version.md)    | 1.0           | byte          | This is not the actual version of the AWDL protocol.    |
| 0x02      | [AF Subtype](subtype.md) | --            | byte          | --                                                      |
| 0x03      | Reserved                 | 0x00          | byte          | --                                                      |
| 0x04-0x07 | Phy TX Time              | --            | 32bit Integer | The time the frame was transmitted at a hardware level. |
| 0x08-0xC  | Target TX Time           | --            | 32bit Integer | The time the frame was crafted, by the driver.          |

## Body

The body of the AFs is made of TLVs, which will be described in the following chapter.
