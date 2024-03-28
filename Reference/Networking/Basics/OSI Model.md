[OSI model - Wikipedia](https://en.wikipedia.org/wiki/OSI_model)

A conceptual model to describe the theoretical aspects of network communication.

The model is composed of layers. Each layer has its own responsibilities and data unit, called a protocol data unit (PDU).

PDU == unit of information transmitted at a particular layer in the OSI model.

[Protocol data unit - Wikipedia](https://en.wikipedia.org/wiki/Protocol_data_unit)


| Layer | Name               | Description                                                                                                                                                                                                                                                                                                                              |
| ----- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7     | Application Layer  | Defines how a human or human controlled software interacts with the network.<br><br>PDU = "data"<br><br>Example: defines how a web browser interacts with the network stack                                                                                                                                                              |
| 6     | Presentation Layer | Responsible for transforming data from the layer below it into a format that can be presented to the user in the application layer.<br><br>PDU = "data"<br><br>Example: encryption/decryption, compression/decompression, etc.                                                                                                           |
| 5     | Session Layer      | Implements protocols that initiate, maintain, and terminate connections between computers - i.e. sessions.<br><br>PDU = "data"                                                                                                                                                                                                           |
| 4     | Transport Layer    | Responsible for ensuring that data gets from A to B in order and on time. Implements error handling<br><br>PDU => TCP = "segments", UDP = "datagrams"                                                                                                                                                                                    |
| 3     | Network Layer      | Concerned with ensuring its PDU gets to it's destination when traveling between networks. Includes routing and broadcasting.<br><br>Think routers and IP addresses.<br><br>PDU = "packets"                                                                                                                                               |
| 2     | Data Link Layer    | Concerned with transferring data between hosts on the same network. Implements error handling. <br><br>Two sub-layers:<br>1. Media Access Control (MAC) - handle device to device communication (think MAC address)<br>2. Logical Link Layer (LLC) - rests on top of MAC and provides flow control/error handling.<br><br>PDU = "frames" |
| 1     | Physical Layer     | Defines how the signal is transferred physically from device to device, such as air waves over WiFi, electronic pulses over Ethernet, light pulses of optical connections, etc.<br><br>Transforms digital bits into physical transmission and back.<br><br>PDU = "bits"                                                                  |
Encapsulation is the process of packaging up the data of a given layer for consumption by the layer above it. This works in reverse, as well.

This is a conceptual model and is not implemented precisely as described in "the real world."