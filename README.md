# Kivanet Miner

A powerful bot to automate mining, task completion, and bulk registration on Kivanet.

## **Features**

- ✅ **Auto Sign-in**
- ✅ **Auto Mining**
- ✅ **Auto Complete Tasks**
- ✅ **Auto-run every 12-12.2 hours**
- ✅ **Multi-account Support**
- ✅ **Proxy Support**
- ✅ **Bulk Register New Accounts**

---

## Prerequisites

Before running the bot, make sure you have:

- Node.js (v16 or higher)
- A valid Kivanet account(s) (register [here](https://kivanet.com/register.html?code=D5Y75I))
- Properly configured `data.txt` file

## Setup & Usage

### 1. Installation

Clone this repository and install dependencies:

```bash
git clone https://github.com/itsnodrops/avik-net-bot.git
cd avik-net-bot
npm install
```

### 2. Running the Bot

Add your OpenLoop account credentials to the `data.txt` file with the following format:

> `email1@mail.com,password1` \
> `email2@mail.com,password2`

```bash
nano data.txt
```

> - Replace `username` and `password` value with your actual credentials

### Optional: Proxy Configuration

To use proxy servers for distribution of requests:

1. Edit `proxies.txt` file in the project root

```bash
nano proxies.txt
```

2. Add one proxy per line in any of these formats:

   HTTP proxies: `host:port:user:pass`
   > Please leave proxies.txt empty if you don't have one.

### Optional: Bulk Registration

To create multiple accounts, save credentials in `registration.txt` (one per line, format: `email,password,invitecode`).

> `email1@mail.com,password1,invteCode` \
> `email2@mail.com,password2,inviteCode`

```bash
 nano registration.txt
```

> - Replace `username`, `password` and `inviteCode` value with your actual credentials

Then, verify the account by following the steps from [here](https://kivanet.com/en.html)

## Project Structure

```
avik-net-bot/
├── index.js            # Main bot script
├── register.js         # Bulk register script
├── package.json        # Project dependencies
├── data.txt            # Accounts log-in credentials storage (important)
├── proxies.txt         # Proxy list (optional)
├── registration.txt    # Bulk-registration accounts credentials storage (optional)
├── tokens.json         # Token storage for authentication
└── src
    ├── banner.js    # Dashboard banner configuration
    ├── colors.js    # Color scheme configuration
    └── ..
```

## Features Explained

- Authenticate using account(s) credentials in `config.json`
- Process accounts with proxy from `proxy.txt` file(if available)
- Fetch signed price data from Stork Oracle API
- Validate and submit results at regular intervals
- Display real-time validation statistics

## Troubleshooting

- Authentication Error: Ensure your username and password are correct in config.json
- Bot Fails to Start: Check if config.json is properly formatted
- Token Expired Issues: Delete tokens.json and restart the bot
- Connection Issues: Verify your internet connection and Stork Oracle API availability
- Proxy Errors: Ensure proxies.txt is correctly formatted

## Support & Links

- GitHub: https://github.com/itsnodrops
- Telegram: https://t.me/NoDrops

## Security Notice

Important: Your credentials are sensitive information. Never share them with anyone and ensure `config.json` is properly secured.

## Contributing

Need source code? Feel free to DM me.

## Disclaimer

This bot is provided as-is, without any warranties. Users are responsible for their own actions. Ensure you understand the risks before using this tool.

## License

This project is licensed under the [MIT License](https://github.com/itsnodrops/avik-net-bot/blob/main/LICENSE).

## Donation

If you want to support the development of this project, you can use this referral code:

```
D5Y75I
```

## Join our community:

- [![Telegram](https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Telegram_logo.svg/12px-Telegram_logo.svg.png)](https://t.me/NoDrops) [NoDrops Telegram Channel](https://t.me/NoDrops)
- [![Telegram](https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Telegram_logo.svg/12px-Telegram_logo.svg.png)](https://t.me/NoDropsChat) [NoDrops Telegram Group](https://t.me/NoDropsChat)
