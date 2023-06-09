# Synchronization Tree TLV

The synchronization tree TLV is relevant to the synchronization process of the AWDL protocol. It contains a complete list of sync addresses. The first address is the master of the entire mesh, the second is syncing to that master and the third is syncing to the third. The minimum amount of addresses is technically one, however in reality at least two addresses are contained, with the second address set to zero.

## Structure

| Bytes     | Meaning                           | Value Type |
| --------- | --------------------------------- | ---------- |
| 0x00-0x05 | Master address                    | EUI48      |
| (...)     | Master from the nodes perspective | EUI48      |


