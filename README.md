# APT Repository for deb-test

## Usage

1. Add the GPG key:
```bash
curl -fsSL https://Silica96.github.io/deb-test/public.key | sudo apt-key add -
```

2. Add the repository:
```bash
echo "deb https://Silica96.github.io/deb-test/ stable main" | sudo tee /etc/apt/sources.list.d/deb-test.list
```

3. Update and install:
```bash
sudo apt update
sudo apt install 
```

## Available Packages

- test_1.0-1_all.deb

Last updated: Sat Aug  9 08:42:04 UTC 2025
