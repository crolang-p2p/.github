# CrolangP2P

## Table of contents
- [The CrolangP2P Project](#the-crolangp2p-project)
- [Available CrolangP2P Node implementations](#available-crolangp2p-node-implementations)
- [CrolangP2P Node Usage Examples list](#crolangp2p-node-usage-examples-list)

## The CrolangP2P Project
### Goals
The CrolangP2P Project aims to provide a stable, robust, and exceptionally simple framework for establishing cross-language peer-to-peer (P2P) connections between clients facilitating seamless data exchange.

The clients are known as Crolang Nodes and are implemented in various programming languages, but the logic is agnostic to the language used, meaning that a client does not care about the language of the other client. Nodes just create a P2P connection referencing the ID of the other Node they want to connect to and start exchanging messages.

The project's core focus is on simplicity, offering a framework that minimizes the need for additional expertise and streamlines the P2P connection process. With a minimal setup time of just a few minutes, developers can concentrate on what truly matters: implementing their desired P2P logic.

Additionally, if a direct P2P connection is not possible or not desired, the Broker also allows nodes to exchange messages via WebSocket, using the Broker as a relay.

### How
To initiate connections, Crolang Nodes rely on a well-known intermediary: the Crolang Broker. This scalable architecture, composed of one or more Broker instances, operates transparently to the nodes. Once a P2P connection is established between two peers, data is exchanged directly among said peers, bypassing the Broker.

The P2P connection is possible by using the WebRTC technology.

### Benefits
- Simple: Minimal setup is required. Developers simply import the Crolang Node dependency into their client, specify the ID of the node they wish to connect to, and the connection process is initiated. This streamlined approach minimizes complexity and allows for rapid development.
- Cross-language Transparency: With multiple implementations of the Crolang Node library available in various programming languages, seamless P2P connections can be established between clients regardless of their underlying language. This cross-language compatibility fosters a versatile and interconnected ecosystem.
- Arbitrary Packet Size Transmission: WebRTC imposes a maximum limit on the size of data packets exchanged. CrolangP2P overcomes this limitation by introducing additional mechanisms to handle larger data payloads. This allows developers to transmit packets of any size, providing greater flexibility and enabling the transfer of substantial data volumes.
- Customizable via extensions: The Broker can be easily extended with custom business logic through a modular extension system. This allows you to adapt authentication, authorization, message handling, and more to your specific needs.

## Available CrolangP2P Node implementations
- [JVM (Kotlin + Java)](https://github.com/crolang-p2p/crolang-p2p-node-jvm)
  
## CrolangP2P Node Usage Examples list
- [JVM (Kotlin): examples-kotlin-crolang-p2p-node-jvm](https://github.com/crolang-p2p/examples-kotlin-crolang-p2p-node-jvm)
