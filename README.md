# 0g-guide-da-retriever

![0G-bg-3](https://github.com/user-attachments/assets/8ade706e-7013-4477-9a2c-e93adab9499c)

## Hardware Requirement 
- RAM: 8 gb
- CPU: 2 cores
- BandWidth: 100 Mbps

# Installation
1. **Install dependencies**
   ```bash
   sudo apt-get update
   sudo apt-get install cmake build-essential protobuf-compiler
   ```
2. **Install Rust**
   ```bash
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```
3. **Download the Source code**
   ```bash
   git clone https://github.com/0glabs/0g-da-retriever.git
   ```

# Configuration
|key|value|
|:--|:----|
|`log_level`|Set log level.|
|`grpc_listen_address`|Server listening address.|
|`eth_rpc_endpoint`|JSON RPC node endpoint for the blockchain network.|

# Run
- Build The Source Code
  ```bash
  cargo build --release
  ```
- Run
  ```bash
  ./target/release/retriever --config ./run/config.toml
  ```
