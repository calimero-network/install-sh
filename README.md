# install-sh

Repository with installation scripts for the calimero binaries.  
Calimero binaries are located in the [core](https://github.com/calimero-network/core) repository.

## Quick Install

### meroctl

```bash
curl -sSL https://raw.githubusercontent.com/calimero-network/core/master/install-meroctl.sh | bash
```

### merod

```bash
curl -sSL https://raw.githubusercontent.com/calimero-network/core/master/install-merod.sh | bash
```

## Custom Options

You can pass options by using `bash -s --`:

```bash
# Install a specific version
curl -sSL https://raw.githubusercontent.com/calimero-network/core/master/install-meroctl.sh | bash -s -- --version 0.10.0

# Install to a custom directory
curl -sSL https://raw.githubusercontent.com/calimero-network/core/master/install-meroctl.sh | bash -s -- --install-dir /usr/local/bin
```

Or use environment variables:

```bash
curl -sSL https://raw.githubusercontent.com/calimero-network/core/master/install-meroctl.sh | VERSION=0.10.0 bash
```

## Available Options

| Option | Environment Variable | Description |
|--------|---------------------|-------------|
| `--version VERSION` | `VERSION` | Set the version to install |
| `--install-dir DIR` | `INSTALL_DIR` | Set the installation directory (default: `$HOME/.local/bin`) |
| `--repo REPO` | `REPO` | Set the GitHub repository (default: `calimero-network/core`) |
| `--help` | - | Display help message |
