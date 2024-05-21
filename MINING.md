
# MINING.md

## Mining SlothBlockCoin (SLBC)

Welcome to the mining guide for SlothBlockCoin (SLBC)! This document will help you get started with solo mining SLBC, as there are currently no mining pools available yet. SlothBlockCoin uses the Scrypt hashing algorithm and requires specific configurations to mine effectively.

### Prerequisites

Before you start mining, ensure you have the following:

1. **SlothBlockCoin Core Wallet**: You need to have the SlothBlockCoin Core wallet installed and configured. (See [our releases](https://github.com/Slothblock/slothblockcoin/releases/latest))

2. **Mining Software**: We recommend using either Nevermore Miner or CPUMiner.

## Step-by-Step Mining Guide

#### Step 1: Download and Install the SlothBlockCoin Core Wallet

1. **Download the Wallet**: Visit our [releases page](https://github.com/Slothblock/slothblockcoin/releases/latest) and download the latest version of the SlothBlockCoin Core wallet.

2. **Extract the Files**: Extract the downloaded ZIP file to a location of your choice.

3. **Launch the Wallet**: Open the `bin` folder and double-click `slothblockcoin-qt.exe` to launch the wallet. This will start your SlothBlockCoin node.

**Note**: The wallet and the daemon (`slothblockcoind.exe`) both launch a node. For most users, using the wallet (`slothblockcoin-qt.exe`) is recommended. You cannot use both at the same time.

#### Step 2: Configure Your Wallet

To mine SLBC, you need to configure your SlothBlockCoin Core wallet with the correct RPC settings. This involves creating and editing the `slothblockcoin.conf` file located in your SlothBlockCoin data directory.

**Configuration File Location**:

- **Windows**: `C:\Users\<YourUsername>\AppData\Roaming\SlothBlockCoin\slothblockcoin.conf`

**Note**: The `slothblockcoin.conf` file probably won't exist at first. You will need to create it manually.

**Example Configuration**:

```plaintext

rpcuser=myusername

rpcpassword=mypassword

rpcallowip=10.0.0.0/24

server=1

daemon=1

```

- `myusername` and `mypassword` are placeholders. Replace them with your own credentials.

- `rpcallowip` allows connections from your local network.
- **IMPORTANT:** After configuring, restart your wallet/node.

#### Step 3: Download and Configure Mining Software

**Nevermore Miner**:

- Download Nevermore Miner from [this link](https://github.com/brian112358/nevermore-miner).

**CPUMiner**:

- Download CPUMiner from [this link](https://github.com/pooler/cpuminer).

#### Step 4: Start Mining

**Using CPUMiner**:

1. Open a command prompt.

2. Navigate to the directory where `minerd.exe` is located.

3. Run the following command:

```plaintext

minerd.exe -o http://127.0.0.1:44345 -O myusername:mypassword --no-getwork --coinbase-addr=(YOUR ADDRESS) --no-stratum --no-redirect

```

Replace `myusername` and `mypassword` with the credentials you set in your `slothblockcoin.conf` file. Replace `(YOUR ADDRESS)` with your SlothBlockCoin wallet address.

**Using Nevermore Miner**:

1. Open a command prompt.

2. Navigate to the directory where `ccminer.exe` is located.

3. Run the following command:

```plaintext

ccminer.exe --no-getwork -a scrypt -o http://127.0.0.1:44345 -u myusername -p mypassword --coinbase-addr=(YOUR ADDRESS) --no-getwork --no-longpoll --no-stratum --no-extranonce

```

Replace `myusername` and `mypassword` with the credentials you set in your `slothblockcoin.conf` file. Replace `(YOUR ADDRESS)` with your SlothBlockCoin wallet address.

### Additional Miner Options

There are likely more mining software options out there that could work with SlothBlockCoin. If you find any other viable miners, please email us at [info@slothblock.com](mailto:info@slothblock.com) to share your findings.

### Important Notes

- Ensure your SlothBlockCoin Core wallet or node is running and fully synchronized with the network.

- The RPC URL should point to your local node, typically `http://127.0.0.1:44345`.

- Do not expose your RPC ports to the public internet for security reasons.

### Conclusion

Solo mining SlothBlockCoin can be a rewarding experience, especially as the community grows. By following this guide, you should be able to set up your mining environment and start contributing to the SlothBlockCoin network. Happy mining!

For more information, visit our [website](http://slothblock.com) or join our [subreddit](https://www.reddit.com/r/slothblock/).
