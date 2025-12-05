 ZYNTRAQ VPN — Chrome Extension

A lightweight Chrome extension that securely retrieves VPN server information from a private backend.  
No sensitive data (IP addresses, keys, or server configs) is stored inside the extension or uploaded to GitHub.

## 🚀 Features

- Fetches VPN server status from a secure backend endpoint  
- Clean and simple popup interface  
- Privacy-first architecture  
- Fully compatible with Chrome Manifest V3  


- `config.json` is intentionally ignored via `.gitignore`
- Only `config.example.json` is included in the repository
- No real VPN server data is stored inside the public codebase

## 📁 Project Structure

```
vpn-extension/
│
├── manifest.json
├── background.js
├── config.example.json
├── popup/
│   ├── popup.html
│   ├── popup.js
│   └── popup.css
├── README.md
└── .gitignore
```

## 🧩 How It Works

1. The extension loads `config.json` locally when it runs.  
2. It reads `vpnApiUrl` from that file.  
3. It requests VPN status data from your backend via HTTPS.  
4. Results appear in the popup UI.  


