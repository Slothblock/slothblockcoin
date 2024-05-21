# SlothBlockCoin Snap Packaging

Commands for building and uploading a SlothBlockCoin Core Snap to the Snap Store. Anyone on amd64 (x86_64), arm64 (aarch64), or i386 (i686) should be able to build it themselves with these instructions. This would pull the official SlothBlockCoin binaries from the releases page, verify them, and install them on a user's machine.

## Building Locally
```
sudo apt install snapd
sudo snap install --classic snapcraft
sudo snapcraft
```

### Installing Locally
```
snap install \*.snap --devmode
```

### To Upload to the Snap Store
```
snapcraft login
snapcraft register slothblockcoin-core
snapcraft upload \*.snap
sudo snap install slothblockcoin-core
```

### Usage
```
slothblockcoin-unofficial.cli # for slothblockcoin-cli
slothblockcoin-unofficial.d # for slothblockcoind
slothblockcoin-unofficial.qt # for slothblockcoin-qt
slothblockcoin-unofficial.test # for test_slothblockcoin
slothblockcoin-unofficial.tx # for slothblockcoin-tx
```

### Uninstalling
```
sudo snap remove slothblockcoin-unofficial
```