# Danom Site Testnet - Get NOM Tokens

## 📌 Minimum Requirements:
- ✅ **CPU:** 4 Cores
- ✅ **RAM:** 8 GB
- ✅ **Storage:** 10 GB HDD

## 📌 Recommended Requirements:
- ✅ **CPU:** 8 Cores
- ✅ **RAM:** 16 GB
- ✅ **Storage:** 40 GB HDD

## 🔹 Step 1: Create an Account
1. Register at [Hugging Face](https://huggingface.co/join)
2. Verify your email
3. Go to your profile settings
4. Navigate to **Access Token**
5. Click **+ Create New Token**
6. Enter a name and create the token
7. Copy your API key (Save it!)

## 🔹 Step 2: Setup on VPS
Run the following commands step by step:
```bash
sudo apt update && sudo apt install -y wget curl tar screen

wget https://github.com/DanomSite/release/releases/download/v4/DanomV4.tar.gz && tar -xvzf DanomV4.tar.gz

cd Danom

curl -fsSL 'https://testnet.danom.site/install.sh' | bash

echo '{"wallet": "0xYOUR_WALLET_ADDRESS", "pool_list": "YOUR_POOL_LIST"}' > wallet_config.json
```
Replace:
- `0xYOUR_WALLET_ADDRESS` → Your **0x wallet address**
- `YOUR_POOL_LIST` → Your **Hugging Face API Key**

## 🔹 Step 3: Start the Worker
```bash
screen -S danom

./danom
```
To detach screen: `CTRL + A + D`

To reattach screen: `screen -r danom`

## 🔹 Claim NOM Tokens (No Fee!)
[Claim NOM](https://testnet.danom.site/)

## 🔹 Swap NOM to MON
[Ambient Monad Swap](https://testnet.danom.site/)

## 🔹 Documentation
[Danom Testnet Docs](https://testnet.danom.site/docs/how-it-work/howitwork)

📌 **Note:** Soon, NOM tokens will be swappable to **DANOM Mainnet!**
