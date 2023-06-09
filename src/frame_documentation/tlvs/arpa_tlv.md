# Arpa TLV

The arpa tlv is one out of three DNS related TLVs. It's used for reverse DNS, since it used to contain the hostname of the peer, which today no longer is the actual hostname of the peer, but a random UUID. This change didn't affect the structure of the TLV.

## Structure

| Byte(s)        | Meaning  | Default Value | Value Type             |
| -------------- | -------- | ------------- | ---------------------- |
| 0x00           | Flags    | 0x03          | 8bit Integer           |
| 0x01+??        | Hostname | --            | [String](../string.md) |
| Last two bytes | Domain   | 0xC000        | [Domain](../domain.md) |

 
