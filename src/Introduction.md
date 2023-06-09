# Introduction

AWDL(**A**pple **W**ireless **D**irect **L**ink) is a protocol, for wireless P2P communication. AWDL is designed to be low latency and high bandwidth, while requiring only one chip for AWDL and "normal" WiFi.

## Contents

In these docs, you will partialy find an explanation for the AWDL frame format, as well as an explanation for the operation of the AWDL protocol. A refrence implementation is available, in the shape of the [awdl-frame-parser](https://crates.io/crates/awdl-frame-parser) crate, which was built by me, so expect refrences to it throughout the docs. Lastly there is a section for bugs found in the AWDL protocol itself.

- [Terminology](./Terminology.md)

- Frame Documentation

## Contributing

If you want to contribute in researching the AWDL protocol further you can support us, by submiting capture files of AWDL traffic. Please send you capture files to [frostie@fnordeingang.de](mailto:frostie@fnordeingang.de)

### Linux

Under Linux you will have todo the following things.

- Set your NIC into monitor mode:```sudo airmon-ng start <NAME OF YOUR NIC>```

- Set your NIC to channel 44 OR 6: ```sudo iw dev <NAME OF YOUR MONITOR IF> set channel (6|44)```

- Start capturing with tshark: ```tshark -i <NAME OF YOUR MONITOR IF> -w output.pcapng```

## Credits

The entire initial research about AWDL was done by the [Open Wireless Link](https://owlink.org/) project, so props to them, since the largest portion of the information compiled here is recycled from their publications. More specifically, Milan Stute's dissertation is used as a resource.

- [Publications | Open Wireless Link](https://owlink.org/publications/)

- https://tuprints.ulb.tu-darmstadt.de/11457/1/dissertation_milan-stute_2020.pdf
