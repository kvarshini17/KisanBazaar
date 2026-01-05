# 🌾 KisanBazaar - Direct Farmer to Consumer Marketplace

A web-based MVP platform enabling **direct farmer-to-consumer trade** with **MSP transparency** and **government scheme awareness**.

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Flask](https://img.shields.io/badge/Flask-3.0-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 🎯 Problem Statement

Indian farmers often face:
- **Middlemen exploitation** reducing their profits
- **Lack of MSP awareness** leading to unfair pricing
- **Limited market access** to sell directly to consumers
- **Unawareness of government schemes** and benefits

## 💡 Solution

**KisanBazaar** provides:
- ✅ Direct farmer-to-consumer marketplace
- ✅ Real-time MSP comparison for every crop
- ✅ Government schemes information
- ✅ Transparent and fair pricing

---

## 🏗️ System Architecture

```
Browser (Frontend)
   ↓ HTTP Requests
Flask Server (Backend Logic)
   ↓ SQL Queries
SQLite Database
```

---

## 🚀 Quick Start

### Prerequisites
- Python 3.9 or higher
- pip (Python package manager)

### Installation

1. **Clone/Navigate to the project**
```bash
cd rsr
```

2. **Create virtual environment** (recommended)
```bash
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # Linux/Mac
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the application**
```bash
python app.py
```

5. **Open in browser**
```
http://localhost:5000
```

---

## 📄 Pages & Features

| Page | Route | Description |
|------|-------|-------------|
| Home | `/` | Landing page with platform overview |
| Farmer Login | `/farmer/login` | Farmer authentication |
| Farmer Register | `/farmer/register` | New farmer registration |
| Farmer Dashboard | `/farmer/dashboard` | Add crops, view listings, MSP comparison |
| Marketplace | `/marketplace` | Browse all available crops |
| Order | `/order/<crop_id>` | Place demo orders |
| MSP Rates | `/msp` | View all MSP rates |
| Govt Schemes | `/schemes` | Government schemes information |

---

## 👥 User Roles

### 👨‍🌾 Farmer
- Register/Login to account
- List crops with price and quantity
- See instant MSP comparison
- Track orders received

### 🛒 Consumer
- Browse marketplace (no login required)
- Filter by crop, location
- View MSP status for transparency
- Place demo orders

---

## 🔑 Demo Credentials

**Farmer Login:**
- Name: `Rajesh Kumar`
- Password: `farmer123`

---

## 📊 Database Schema

### Tables
1. **farmers** - Farmer accounts
2. **crops** - Crop listings
3. **orders** - Order records
4. **msp** - MSP rates
5. **schemes** - Government schemes

---

## 🌟 Core Feature: MSP Comparison Engine

```python
if farmer_price >= msp_price:
    status = "Above MSP"  # ✅ Fair Price
else:
    status = "Below MSP"  # ⚠️ Warning
```

This comparison is shown:
- When farmer adds a crop
- On farmer dashboard
- In consumer marketplace

---

## 🏛️ Government Schemes Included

- PM-KISAN
- PMFBY (Crop Insurance)
- Soil Health Card
- Kisan Credit Card
- e-NAM
- PM Krishi Sinchai Yojana

---

## 📁 Project Structure

```
rsr/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # This file
├── kisanbazaar.db        # SQLite database (auto-created)
├── static/
│   └── css/
│       └── style.css     # Custom styles
└── templates/
    ├── base.html             # Base template
    ├── home.html             # Home page
    ├── farmer_login.html     # Farmer login
    ├── farmer_register.html  # Farmer registration
    ├── farmer_dashboard.html # Farmer dashboard
    ├── marketplace.html      # Consumer marketplace
    ├── order.html            # Order page
    ├── order_success.html    # Order confirmation
    ├── schemes.html          # Government schemes
    └── msp_info.html         # MSP rates
```

---

## 🔮 Future Enhancements

- [ ] Payment gateway integration (UPI)
- [ ] Mobile app version
- [ ] AI-based price prediction
- [ ] Multi-language support
- [ ] Real-time order tracking
- [ ] SMS/WhatsApp notifications
- [ ] Government API integration for live MSP

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | HTML, CSS, Bootstrap 5, Jinja2 |
| Backend | Python, Flask |
| Database | SQLite |
| Icons | Bootstrap Icons |

---

## 📝 License

MIT License - Feel free to use for hackathons and learning!

---

## 🙏 Acknowledgments

- Government of India MSP data
- Bootstrap for UI components
- Flask community

---

**Made with ❤️ for Indian Farmers**
