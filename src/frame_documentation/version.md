# AWDL Version Format

In the AWDL frame format a version is expressed as a one byte value, of which the upper half indicates the major version and the lower half the minor version.

| bits | meaning |
| ---- | ------- |
| 0-3  | minor   |
| 4-7  | major   |

For example a version of 3.14 would be expressed as ```0011_1110```.
