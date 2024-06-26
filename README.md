<h1 align="center">
<img src="https://slothblock.info/images/hdlogo.png" alt="SlothBlockCoin" width="300"/>
<br/><br/>
SlothBlockCoin Core [SLBC]
</h1>

<div align="center">



</div>


SlothBlockCoin is a community-driven cryptocurrency that was inspired by a Sloth meme. The SlothBlockCoin Core software allows anyone to operate a node in the SlothBlockCoin blockchain networks and uses the Scrypt hashing method for Proof of Work. It is adapted from Bitcoin Core and other cryptocurrencies.

For information about the default fees used on the SlothBlockCoin network, please
refer to the [fee recommendation](doc/fee-recommendation.md).

**Website:** [slothblock.com](https://slothblock.com)

## Usage 💻

To start your journey with SlothBlockCoin Core, see the [installation guide](INSTALL.md) and the [getting started](doc/getting-started.md) tutorial.

The JSON-RPC API provided by SlothBlockCoin Core is self-documenting and can be browsed with `slothblockcoin-cli help`, while detailed information for each command can be viewed with `slothblockcoin-cli help <command>`. Alternatively, see the [Bitcoin Core documentation](https://developer.bitcoin.org/reference/rpc/) - which implement a similar protocol - to get a browsable version.

### Ports

SlothBlockCoin Core by default uses port `44346` for peer-to-peer communication that
is needed to synchronize the "mainnet" blockchain and stay informed of new
transactions and blocks. Additionally, a JSONRPC port can be opened, which
defaults to port `44345` for mainnet nodes. It is strongly recommended to not
expose RPC ports to the public internet.

| Function | mainnet | testnet | regtest |
| :------- | ------: | ------: | ------: |
| P2P      |   44346 |   17264 |   15262 |
| RPC      |   44345 |   17263 |   15261 |

## Ongoing development - Moon plan 🌒

SlothBlockCoin Core is an open source and community driven software. The development
process is open and publicly visible; anyone can see, discuss and work on the
software.

Main development resources:

* [GitHub Projects](https://github.com/Slothblock/slothblockcoin/projects) is used to
  follow planned and in-progress work for upcoming releases.
* [GitHub Discussion](https://github.com/Slothblock/slothblockcoin/discussions) is used
  to discuss features, planned and unplanned, related to both the development of
  the SlothBlockCoin Core software, the underlying protocols and the SLBC asset.  
* [SlothBlockCoin subreddit](https://www.reddit.com/r/slothblock/)

### Version strategy
Version numbers are following ```major.minor.patch``` semantics.

### Branches
There are 3 types of branches in this repository:

- **master:** Stable, contains the latest version of the latest *major.minor* release.
- **maintenance:** Stable, contains the latest version of previous releases, which are still under active maintenance. Format: ```<version>-maint```
- **development:** Unstable, contains new code for planned releases. Format: ```<version>-dev```

*Master and maintenance branches are exclusively mutable by release. Planned*
*releases will always have a development branch and pull requests should be*
*submitted against those. Maintenance branches are there for **bug fixes only,***
*please submit new features against the development branch with the highest version.*

## Contributing 🤝

If you find a bug or experience issues with this software, please report it
using the [issue system](https://github.com/Slothblock/slothblockcoin/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5Bbug%5D+).

Please see [the contribution guide](CONTRIBUTING.md) to see how you can
participate in the development of SlothBlockCoin Core. There are often
[topics seeking help](https://github.com/Slothblock/slothblockcoin/labels/help%20wanted)
where your contributions will have high impact and get very appreciation. wow.

## Communities 🚀🍾

You can join the communities on different social media.
To see what's going on, meet people & discuss, find the latest meme, learn
about SlothBlockCoin, give or ask for help, to share your project.

Here are some places to visit:

* [SlothBlockCoin subreddit](https://www.reddit.com/r/slothblock/)
* [SlothBlockCoin Twitter](https://twitter.com/SlothBlockCoin)

## Frequently Asked Questions ❓

Do you have a question regarding SlothBlockCoin? An answer is perhaps already in the
[Whitepaper](https://www.slothblock.com/brilliant-blueprint).

## License ⚖️
SlothBlockCoin Core is released under the terms of the MIT license. See
[COPYING](COPYING) for more information or see
[opensource.org](https://opensource.org/licenses/MIT)
