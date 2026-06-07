# 🌾 Kisan Mitra

> *AI-Powered Agricultural Monitoring & Profit Intelligence Platform*

[![SIH 2024](https://img.shields.io/badge/Smart%20India%20Hackathon-Round%202%20Selected-FF6B00?style=flat&logo=india&logoColor=white)]()
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg)](CONTRIBUTING.md)

---

<div align="center">

### 🏆 Selected in Round 2 — Smart India Hackathon (SIH)

*Empowering farmers with AI-driven insights, real-time monitoring, and intelligent profit planning*

</div>

---

## 📖 Overview

**Kisan Mitra** (*Friend of the Farmer*) is a full-stack AI agricultural platform designed to modernize Indian farming. It combines real-time crop monitoring, soil and weather intelligence, disease detection, and a first-of-its-kind **Profit Planner Engine** — giving farmers and agri-businesses the tools to make data-driven decisions that directly improve yield and income.

> Built with a mission: bridge the technology gap in Indian agriculture and put actionable intelligence in every farmer's hands.

---

## 🏅 Smart India Hackathon — Achievement

```
 ╔══════════════════════════════════════════════════════════╗
 ║         🇮🇳  SMART INDIA HACKATHON  —  SIH 2024          ║
 ║                                                          ║
 ║   Status   :  ✅  Selected in Round 2                    ║
 ║   Category :  Agriculture & Rural Development            ║
 ║   Theme    :  AI-Driven Smart Farming Solutions          ║
 ╚══════════════════════════════════════════════════════════╝
```

Kisan Mitra was evaluated among thousands of national submissions and advanced to **Round 2** of the Smart India Hackathon for its innovative approach to agricultural AI, particularly the Profit Planner module and real-time crop health monitoring system.

---

## ✨ Platform Features

### 🌟 Flagship Innovation

#### 💰 Profit Planner — *Unique Feature*
> The core differentiator of Kisan Mitra. No other platform does this.

The **Profit Planner Engine** is an AI-powered decision system that:
- Ingests **farming datasets** (soil type, crop history, seasonal data, land size, input costs)
- Analyses **agricultural product data** (seeds, fertilizers, pesticides, market prices)
- Runs predictive models to identify the **most profitable crop combinations**
- Generates a **step-by-step profit improvement roadmap** for each farmer
- Recommends **when to sell, what to grow, and how to cut input costs**

```
INPUT DATASET             AI ENGINE              OUTPUT
─────────────────         ──────────────         ────────────────────────
Soil data          ──►                    ──►   Best crop recommendation
Crop history       ──►   Profit Planner   ──►   Expected ROI per acre
Market prices      ──►   (ML + Rules)     ──►   Cost reduction tips
Weather patterns   ──►                    ──►   Selling window alerts
Product costs      ──►                    ──►   Profit improvement plan
```

---

### 🌱 Core Agricultural Features

| Module | Description |
|---|---|
| 🛰️ **Crop Monitoring** | Real-time crop health tracking using sensor & satellite data |
| 🌡️ **Soil Intelligence** | Soil moisture, pH, nutrient level monitoring with alerts |
| ☁️ **Weather Integration** | Hyperlocal weather forecasting and farm-specific advisories |
| 🔬 **Disease Detection** | AI image recognition for early crop disease and pest detection |
| 💧 **Irrigation Manager** | Smart irrigation scheduling based on soil and weather data |
| 💰 **Profit Planner** | Dataset-driven profit optimization engine *(Unique Feature)* |
| 📦 **Market Linkage** | Live mandi prices, demand forecasting, and direct buyer connect |
| 📋 **Farm Dashboard** | Unified view of all farm metrics, alerts, and recommendations |
| 🌾 **Crop Calendar** | AI-generated sowing, fertilizing, and harvesting schedule |
| 📱 **Farmer App** | Mobile-first interface with regional language support |
| 🤖 **AI Advisory** | Personalized chatbot advisor for crop and finance queries |
| 📊 **Yield Prediction** | ML models to forecast expected yield before harvest |

---

## 🛠️ Tech Stack

```
Frontend         →  Next.js / React Native, Tailwind CSS
Backend          →  Node.js, Express.js, Python (ML services)
Database         →  MongoDB, PostgreSQL (farm datasets)
AI / ML          →  TensorFlow / PyTorch, Scikit-learn, OpenAI API
Computer Vision  →  OpenCV (disease detection)
IoT Integration  →  MQTT Protocol, Sensor APIs
Weather API      →  OpenWeatherMap / IMD Integration
Maps & GIS       →  Mapbox / Google Maps API
Auth             →  JWT, OTP-based (for rural accessibility)
Storage          →  AWS S3 / Cloudinary
Deployment       →  Vercel (frontend), AWS EC2 / Railway (backend)
```

---

## 📁 Project Structure

```
kisan-mitra/
├── app/                         # Next.js App Router
│   ├── (auth)/                  # Login, OTP auth
│   ├── dashboard/               # Farm overview dashboard
│   ├── profit-planner/          # 💰 Profit Planner module
│   ├── crop-monitoring/         # Real-time crop health
│   ├── disease-detection/       # AI image scan
│   ├── market/                  # Mandi prices & market
│   ├── weather/                 # Weather advisory
│   └── advisory/                # AI chatbot advisor
├── ml-services/                 # Python ML microservices
│   ├── profit_engine/           # Profit Planner core model
│   ├── disease_model/           # Crop disease CNN model
│   └── yield_predictor/         # Yield forecasting model
├── components/                  # Reusable UI components
├── lib/                         # Utilities and helpers
├── models/                      # Database schemas
├── api/                         # REST API routes
├── public/                      # Static assets
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

- Node.js `v18+`
- Python `3.10+`
- MongoDB (local or Atlas)
- OpenAI API key
- OpenWeatherMap API key

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/kisan-mitra.git
cd kisan-mitra

# 2. Install Node dependencies
npm install

# 3. Install Python ML dependencies
cd ml-services
pip install -r requirements.txt
cd ..

# 4. Set up environment variables
cp .env.example .env.local
# Fill in your API keys (see below)

# 5. Run the development server
npm run dev

# 6. Run ML services (separate terminal)
cd ml-services
python app.py
```

Open [http://localhost:3000](http://localhost:3000) to view the platform.

---

## 🔐 Environment Variables

```env
# App
NEXT_PUBLIC_APP_URL=http://localhost:3000

# MongoDB
MONGODB_URI=your_mongodb_connection_string

# Authentication
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000

# AI
OPENAI_API_KEY=your_openai_api_key

# Weather
OPENWEATHER_API_KEY=your_openweather_api_key

# Maps
NEXT_PUBLIC_MAPBOX_TOKEN=your_mapbox_token

# Storage
AWS_ACCESS_KEY=your_aws_access_key
AWS_SECRET_KEY=your_aws_secret_key
AWS_BUCKET_NAME=your_bucket_name
```

---

## 🧠 Profit Planner — How It Works

```
STEP 1 — DATA INGESTION
  └─ Farmer uploads / inputs: land size, soil report, past crops,
     water availability, budget, preferred crop type

STEP 2 — PRODUCT DATASET ANALYSIS
  └─ System fetches: seed prices, fertilizer costs, pesticide costs,
     current mandi rates, demand trends, seasonal market patterns

STEP 3 — AI PROFIT MODELING
  └─ ML model runs multi-variable optimization:
     Expected Revenue - Total Input Cost = Projected Profit
     Models tested: Random Forest, XGBoost, Linear Regression

STEP 4 — PROFIT IMPROVEMENT PLAN
  └─ Output: Top 3 recommended crops with projected ROI
     Cost-cutting suggestions per input category
     Optimal selling month based on price forecasting
     Government scheme eligibility matched to farmer profile

STEP 5 — CONTINUOUS LEARNING
  └─ Farmer outcomes fed back into model for regional accuracy
```

---

## 🗺️ Roadmap

- [x] Farm monitoring dashboard
- [x] Soil & weather intelligence
- [x] AI disease detection (image-based)
- [x] Profit Planner v1 (core engine)
- [x] Mandi price integration
- [x] SIH Round 2 submission
- [ ] Profit Planner v2 (real-time market feed)
- [ ] IoT sensor hardware integration
- [ ] Regional language support (Hindi, Tamil, Telugu)
- [ ] Offline mode for low-connectivity areas
- [ ] Government scheme auto-matching
- [ ] Mobile app (React Native)
- [ ] Farmer community & peer network

---

## 📸 Screenshots

> *(Add screenshots or demo GIF here)*

```
/docs/screenshots/dashboard.png
/docs/screenshots/profit-planner.png
/docs/screenshots/disease-detection.png
/docs/screenshots/crop-calendar.png
```

---

## 🤝 Contributing

Contributions are welcome from developers, data scientists, and agricultural domain experts!

```bash
# Fork → Branch → Commit → PR
git checkout -b feature/your-feature-name
git commit -m "feat: add your feature"
git push origin feature/your-feature-name
```

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Kishore** — [GitHub](https://github.com/your-username) · [LinkedIn](https://linkedin.com/in/your-profile)

---

## 🙏 Acknowledgements

- **Smart India Hackathon (SIH)** — for the platform to bring this vision to national attention
- **Indian Council of Agricultural Research (ICAR)** — for agricultural datasets and domain reference
- **OpenWeatherMap & IMD** — for weather data APIs
- All farmers and agricultural experts who provided feedback during development

---

<div align="center">

🌾 *Kisan Mitra — Because every farmer deserves smart technology* 🌾

Built with ❤️ for Bharat's farmers

</div>
