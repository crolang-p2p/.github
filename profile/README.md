# CrolangP2P
Easy cross-language framework for P2P communication.

## Table of Contents
- [The CrolangP2P Project](#the-crolangp2p-project)
- [How it works](#how-it-works)
- [Available CrolangP2P Node implementations](#available-crolangp2p-node-implementations)
- [Usage Examples](#usage-examples)

## The CrolangP2P Project
CrolangP2P is a simple, robust framework for cross-language peer-to-peer (P2P) connections. Clients (“Crolang Nodes”) libraries can be easily integrated into your project and connect using only the ID of the target node, exchanging messages directly via P2P or via WebSocket using the [Crolang Broker](https://github.com/crolang-p2p/crolang-p2p-broker) as relay. The framework manages the connection an you can focus on what matters most: your project's logic.

- **Simplicity:** Minimal setup—just import the Node library, specify the peer ID, and connect.
- **Cross-language:** [Multiple Node implementations](#available-crolangp2p-node-implementations) allow seamless P2P between different languages.
- **No packet size limits:** Large data exchange is supported.
- **Extensible:** The Broker supports modular extensions for authentication, authorization, message handling, and more.

Nodes connect through the [Crolang Broker](https://github.com/crolang-p2p/crolang-p2p-broker), which acts as a rendezvous point: it helps nodes discover each other and establish direct WebRTC connections.

## Available CrolangP2P Node implementations
- [JVM (Kotlin + Java)](https://github.com/crolang-p2p/crolang-p2p-node-jvm)

More implementations will be available in the future.

## Usage Examples
- [JVM (Kotlin): examples-kotlin-crolang-p2p-node-jvm](https://github.com/crolang-p2p/examples-kotlin-crolang-p2p-node-jvm)
- [JVM (Java): examples-java-crolang-p2p-node-jvm](https://github.com/crolang-p2p/examples-java-crolang-p2p-node-jvm)
