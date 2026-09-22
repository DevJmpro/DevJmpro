![JM Pro API](./banner.jpg)

<div align="center">

# JM Pro API
  
Build automated trading workflows with real-time order execution, live market feeds, and portfolio APIs.

JM Pro API gives developers direct programmatic access to India's stock markets for executing your strategies across NSE and BSE.

<br/>

[![Python SDK](https://img.shields.io/badge/Python_SDK-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/DevJmpro/PyJmproAPI)
[![Java SDK](https://img.shields.io/badge/Java_SDK-E76F00?style=for-the-badge&logo=openjdk&logoColor=white)](https://github.com/DevJmpro/JavaJmproAPI)
[![Go SDK](https://img.shields.io/badge/Go_SDK-00ACD7?style=for-the-badge&logo=go&logoColor=white)](https://github.com/DevJmpro/GoJmproAPI)
[![Node.js SDK](https://img.shields.io/badge/Node.js_SDK-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://github.com/DevJmpro/NodeJsJmproAPI)

</div>

---

## ⚡ What You Can Build

| Capability | Description |
|---|---|
| **Order Management** | Execute the full order lifecycle - up to **9 Orders Per Second** |
| **Live Market Feed** | WebSocket streaming for instruments across NSE & BSE |
| **Historical Data** | Tick-by-tick and OHLCV candle data for backtesting and analysis |
| **Portfolio Management** | Real-time holdings, positions, P&L and margin data |
| **Authentication** | OAuth 2.0 - secure, stateless, daily-session based |

---

## 🚀 Quickstart

**1. Sign up, Create your APP and get your API key**

```
https://developer.jmproapp.com/signup
```

**2. Install the SDK**

```bash
# To install Python SDK
pip install jmpro-python          
# To install Node.js SDK
npm install jmpro-nodejs          
# To install Go SDK
go get github.com/jmpro/jmpro-go 
# To install Java SDK

```

**3. Place your first order**

```python
# Authenticate with JM Pro API
from pyjmproapi import PyJmproAPI

jmpro = PyJmproAPI(api_key="your_api_key")
jmpro.set_access_token("your_access_token")

# Place an order in real-time
jmpro.place_order(
  variety=jmpro.VARIETY_REGULAR,
  exchange=jmpro.EXCHANGE_BSE,
  tradingsymbol="INDEX",
  transaction_type=jmpro.TRANSACTION_TYPE_BUY,
  quantity=1,
  product=jmpro.PRODUCT_CNC,
  price=3000,
  order_type=jmpro.ORDER_TYPE_MARKET,
  validity=jmpro.VALIDITY_DAY)

# → { "order_id": "BX20260323001", "status": "PLACED" }
```

---

## 📦 Repositories

| Repository | Language | Description |
|---|---|---|
| [jmpro-python](https://github.com/DevJmpro/PyJmproAPI) | 🐍 Python | Official Python SDK |
| [jmpro-java](https://github.com/DevJmpro/JavaJmproAPI) | ☕ Java | Official Java SDK |
| [jmpro-go](https://github.com/DevJmpro/GoJmproAPI) | 🐹 Go | Official Go client |
| [jmpro-nodejs](https://github.com/DevJmpro/NodeJsJmproAPI) | 🟩 Node.js | Official Node.js SDK |

---

## 📚 Resources

- 📖 &nbsp;[API Documentation](https://developer.jmproapp.com/docs/)
- 🔑 &nbsp;[Get Your API Key](https://developer.jmproapp.com/signup)
- 📧 &nbsp;[General Enquiries](https://jmproapp.com/contact-us)

---

## 📋 Platform Specs

```
Rate Limit          9 orders/second 
Max Orders/Day      14,000
Auth                OAuth 2.0 (daily session)
```

---

JM Pro API complies with all SEBI and exchange regulations for algorithmic trading in India.  
A **static IP address** is mandatory for all API integrations per NSE/BSE guidelines (effective August 2025).  

---

<div align="center">

**© 2026 JM Pro · Powered by JM Financial**  

</div>
