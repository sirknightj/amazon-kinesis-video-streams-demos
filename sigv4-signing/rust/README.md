# KVS Signaling SigV4 WebSocket Signer

A Rust library and collection of tools for signing WebSocket connections to Amazon Kinesis Video Streams (KVS) Signaling channels using AWS SigV4.

## Prerequisites

- Rust installed on your system (and `cargo`)
- AWS credentials
- Kinesis Video Streams Signaling Channel

## Installation

Clone the repository:
```bash
git clone https://github.com/aws-samples/amazon-kinesis-video-streams-demos.git
cd amazon-kinesis-video-streams-demos/sigv4-signing/rust
```

Then build the package.
```shell
cargo build
```

## Running the examples

For samples 1 and 2, edit the constants in the files, then run:
```shell
cargo run --package kvs_signaling_sigv4_wss_signer --example 1_simple_connect_to_socket_sample
```

For example 3, you can run it straight from the command-line. Run:
```shell
cargo run --package kvs_signaling_sigv4_wss_signer --example 3_signer_using_aws_sdk <channel-name> <MASTER|VIEWER> 
```