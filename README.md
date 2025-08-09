# APT Repository for deb-test

## Installation

```bash
# Add GPG key
curl -fsSL https://Silica96.github.io/deb-test/public.key | sudo apt-key add -

# Add repository
echo "deb https://Silica96.github.io/deb-test/ stable main" | sudo tee /etc/apt/sources.list.d/deb-test.list

# Install package
sudo apt update
sudo apt install test
```

Last updated: Sat Aug  9 08:46:52 UTC 2025
