# AWDL Domain Compression

Domains in AWDL are stored in a "compressed" form. Every Domain is stored as a big endian 16bit Integer.

## Table

| Value  | Domain                |
| ------ | --------------------- |
| 0xC000 | NULL                  |
| 0xC001 | \_airplay.\_tcp.local |
| 0xC002 | \_airplay.\_udp.local |
| 0xC003 | \_airplay             |
| 0xC004 | \_raop.\_tcp.local    |
| 0xC005 | \_raop.\_udp.local    |
| 0xC006 | \_raop                |
| 0xC007 | \_airdrop.\_tcp.local |
| 0xC008 | \_airdrop.\_udp.local |
| 0xC009 | \_airdrop             |
| 0xC00A | \_tcp.local           |
| 0xC00B | \_udp.local           |
| 0xC00C | local                 |
| 0xC00D | ip6.arpa              |
| 0xC00E | ip4.arpa              |
