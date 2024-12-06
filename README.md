## Paste your proxies inside proxy.txt and the token inside tokens.txt


# How to Get Nodepay Token -

1. Open your browser and login to the NODEPAY dashboard.
2. Press `F12` to open the **Inspect Elements** panel.
3. Go to the **Console** tab and paste the following code:
```
localStorage.getItem('np_webapp_token') 
```

4. You will receive your user ID, which looks like this: `"eyJhbG........"`
5. If you can't paste, type `allow pasting` and press Enter.

## Recommended Python Version

It is recommended to use **Python 3.10**.  
[Download Python 3.10 here](https://www.python.org/downloads/release/python-3100/).

## Install Requirements

Run the following command to install the necessary packages:

```
pip install -r requirements.txt
```

## Running the Script

```
python npay-proxy.py
```
## FOR ANDROID

# How to Get NODEPAY User ID Using Android Device

1. Download and install [Kiwi Browser](https://play.google.com/store/apps/details?id=com.kiwibrowser.browser&hl=en).
2. Login to the NODEPAY web and go to the dashboard.
3. Open the **Developer Tools** in the Kiwi browser.
4. Go to the **Console** tab and paste this code:
```
localStorage.getItem('np_webapp_token') 
```

5. If you can't paste, type `allow pasting` and press Enter, then paste the line above.

## Configure Termux

After installing Termux, ensure you have allowed storage permission for Termux (device app) settings.  
Alternatively, run this command in Termux:

```
termux-setup-storage
```

### Install Python 3.10

Run the following commands:

```
pkg update && upgrade
```
```
pkg install tur-repo
```
```
pkg install python-is-python3.10
```
```
pkg install -y rust binutils
```
```
CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')" pip install maturin
```

## Clone This Script
```
git clone https://github.com/ashtrobe/nodepay-farm.git
```