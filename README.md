# APT Repository for deb-test

## Installation

### Add GPG key and repository
```bash
# Modern way (Ubuntu 22.04+, Debian 11+)
curl -fsSL https://Silica96.github.io/deb-test/public.key | sudo gpg --dearmor -o /etc/apt/keyrings/deb-test.gpg
echo "deb [signed-by=/etc/apt/keyrings/deb-test.gpg] https://Silica96.github.io/deb-test/ stable main" | sudo tee /etc/apt/sources.list.d/deb-test.list

# Legacy way (older systems)
curl -fsSL https://Silica96.github.io/deb-test/public.key | sudo apt-key add -
echo "deb https://Silica96.github.io/deb-test/ stable main" | sudo tee /etc/apt/sources.list.d/deb-test.list
```

### Install package
```bash
sudo apt update
sudo apt install test
```

### Install specific version
```bash
# List available versions
apt-cache madison test

# Install specific version
sudo apt install test=VERSION
```

## Available Packages

```
stable|main|amd64: test 1.0-4
stable|main|arm64: test 1.0-4
stable|main|armhf: test 1.0-4
stable|main|i386: test 1.0-4
```

Last updated: Sat Aug  9 09:50:15 UTC 2025
