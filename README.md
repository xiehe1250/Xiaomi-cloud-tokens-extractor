# Xiaomi Cloud Tokens Extractor
[![buymeacoffee_badge](https://img.shields.io/badge/Donate-buymeacoffe-ff813f?style=flat)](https://www.buymeacoffee.com/PiotrMachowski)

This tool/script retrieves tokens for all devices connected to Xiaomi cloud.

You will need to provide Xiaomi Home credentials (_not ones from Roborock app_):
- username (e-mail or Xiaomi Cloud account ID)
- password
- Xiaomi's server region (`cn` - China, `de` - Germany etc.). Leave empty to check all available

In return all of your devices connected to account will be listed, together with their name and IP address.

## Windows
Download and run [token_extractor.exe](https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor/raw/master/token_extractor.exe).

## Docker

Clone this repository:
```bash
git clone https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor.git
```

Go to cloned directory:
```bash
cd Xiaomi-cloud-tokens-extractor
```

Build and run script using docker:
```bash
docker run --rm -it $(docker build -q .)
```

## Other platforms

Install dependencies:
```bash
pip3 install pycryptodome pybase64 requests
```

Download and run script:
```bash
wget https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor/raw/master/token_extractor.py
python3 token_extractor.py
```


<a href="https://www.buymeacoffee.com/PiotrMachowski" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
