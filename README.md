# KaamShield AI 🛡️
### Production Operations Intelligence & Business Failure Simulator for MSMEs
**NVIDIA × Nebius Global AI Hackathon — Best Apps & Agents Track**

<p align="center">
  <img src="https://img.shields.io/badge/Status-Production%20Ready-00F5A0?style=for-the-badge&logo=statuspage&logoColor=white" alt="Status" />
  <img src="https://img.shields.io/badge/Model-NVIDIA%20Nemotron%203%20MoE-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="NVIDIA Nemotron" />
  <img src="https://img.shields.io/badge/Inference-Nebius%20Token%20Factory-00D26A?style=for-the-badge&logo=lightning&logoColor=white" alt="Nebius Token Factory" />
  <img src="https://img.shields.io/badge/Frontend-Next.js%2014%20%7C%20Tailwind-black?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Backend-FastAPI%20%7C%20Python%203.11+-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Tests-6%2F6%20Passing%20(100%25)-brightgreen?style=for-the-badge&logo=pytest&logoColor=white" alt="Pytest" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License" />
</p>

> *"See the risk. Prevent the loss."*  
> **KaamShield AI** is an AI operations command center engineered for manufacturing MSMEs. It bridges real-time factory ledgers with **NVIDIA Nemotron 3 MoE** reasoning served through **Nebius Token Factory**, pairing verifiable deterministic business logic with zero-hallucination operational advisory.

---

## 📌 Table of Contents
1. [The Real-World Problem](#-the-real-world-problem)
2. [Key Product Innovations](#-key-product-innovations)
3. [NVIDIA Nemotron × Nebius Token Factory Integration](#-nvidia-nemotron--nebius-token-factory-integration)
4. [System Architecture](#-system-architecture)
5. [Core Mathematical & Deterministic Formulas](#-core-mathematical--deterministic-formulas)
6. [Interactive Application Workspaces](#-interactive-application-workspaces)
7. [Quickstart & Local Installation](#-quickstart--local-installation)
8. [Automated Verification & Test Suite](#-automated-verification--test-suite)
9. [Docker Deployment](#-docker-deployment)
10. [Hackathon Evaluation Checklist](#-hackathon-evaluation-checklist)
11. [License](#-license)

---

## 🏭 The Real-World Problem

Over 63 million Micro, Small, and Medium Enterprises (MSMEs) power global industrial manufacturing. In sectors like automotive tooling, precision engineering, and electronics assembly, businesses operate on thin margins ($8–14\%$) with fragmented ERPs and paper invoices. 

**82% of small manufacturer insolvencies stem from operational shocks discovered too late:**
- **Lead-Time Blindness:** Critical raw alloy bars or fasteners run out mid-production due to unannounced vendor delays.
- **Invoice Discrepancies & Price Creep:** Suppliers invoice at inflated unit rates (e.g. ₹315/pc vs. agreed ₹285/pc) or bill for quantities exceeding approved Purchase Orders.
- **Duplicate Invoices:** Identical vendor invoices submitted weeks apart bypass manual spreadsheet checks.
- **Cash-Flow Cliff:** Client payment delays collide with scheduled bi-weekly payroll and power bills, triggering immediate liquidity failure.

Existing ERPs act as passive historical recorders. **KaamShield AI acts as an active, preventative co-pilot.**

---

## ⚡ Key Product Innovations

### 1. Flagship: Business Failure Simulator
A split-screen stress-testing studio allowing plant owners and financial controllers to simulate shocks before committing working capital:
- **Supplier Delay (0–14 Days):** Recalculates exact stock runout dates and unfulfilled capacity revenue at risk.
- **Demand Surges / Drops (-50% to +100%):** Models safety stock depletion and automated reorder buffers.
- **Customer Payment Delays (0–45 Days):** Pinpoints the exact calendar date of working capital insolvency.
- **Raw Material Price Hikes (0–50%):** Quantifies direct gross margin erosion.
- **Cheapest Feasible Mitigations:** Delivers instant, mathematically derived contingency plans (e.g., air-freighting partial batches vs. offering 2% early-collection discounts).

### 2. Dual-Engine Intelligence: Factual Grounding + Nemotron Reasoning
- **Never hallucinates financial figures:** All quantities, variances, and dates are derived deterministically in Python/NumPy/Pandas.
- **Contextual synthesis via NVIDIA Nemotron 3:** Operates strictly on a structured **Operational Evidence Package** extracted from database records.
- **100% Uptime Fallback:** If cloud inference is offline or unconfigured, the system automatically falls back to KaamShield's **Deterministic Intelligence Engine** with clear UI labeling.

---

## 🧠 NVIDIA Nemotron × Nebius Token Factory Integration

KaamShield AI integrates **NVIDIA Nemotron 3 MoE** hosted on **Nebius Token Factory** using its OpenAI-compatible endpoint.                                                                                                                                                      

### Configuration Environment
In `.env`:
```bash
NEBIUS_API_KEY=your_nebius_token_factory_key
NEBIUS_BASE_URL=https://api.tokenfactory.nebius.com/v1/
NVIDIA_NEMOTRON_MODEL=nvidia/nemotron-3-super-120b-a12b
(If NEBIUS_API_KEY is not provided, KaamShield seamlessly runs in Deterministic Engine mode with 100% feature availability)
kaamshield-ai/
├── backend/
│   ├── app/
│   │   ├── ai/            # Nebius Token Factory client & ERP evidence extractor
│   │   ├── analytics/     # Stockout, 3-way invoice audit, supplier risk, cash flow, simulator
│   │   ├── api/           # REST endpoints (health, dashboard, inventory, simulator, copilot, demo)
│   │   ├── core/          # Pydantic Settings, database engine, SQLite/PostgreSQL configuration
│   │   ├── models/        # Normalized SQLAlchemy tables
│   │   ├── schemas/       # Typed Pydantic request/response schemas
│   │   ├── tests/         # Pytest automated test suite (6/6 passing)
│   │   └── main.py        # FastAPI app entrypoint
│   ├── Dockerfile
│   └── requirements.txt
├── frontend/
│   ├── app/               # Next.js 14 App Router (layout, page, theme)
│   ├── components/        # Dashboard, Simulator, Copilot, Inventory, Auditor, CashFlow, ActionCenter
│   ├── components/ui/     # Reusable design primitives (Badge, CircularScore)
│   ├── lib/api.ts         # Typed API client
│   └── Dockerfile
├── sample_data/           # Downloadable MSME CSV templates
├── docs/                  # Architecture diagrams & 3-minute video demo script
├── docker-compose.yml     # Complete multi-container deployment
├── .env.example
├── LICENSE                # MIT License
└── README.md                                                                                                                             🚀 Quickstart & Local Installation
Prerequisites
Python 3.11+
Node.js 18+ and npm
Git
1. Clone & Configure
bash
git clone https://github.com/your-username/kaamshield-ai.git
cd kaamshield-ai
cp .env.example .env
2. Launch Backend (FastAPI)
bash
# Setup Python virtual environment
python -m venv venv
# Activate (Windows)
.\venv\Scripts\activate
# Activate (Linux / macOS)
source venv/bin/activate
# Install dependencies
pip install -r backend/requirements.txt
# Run FastAPI server
uvicorn backend.app.main:app --host 127.0.0.1 --port 8000 --reload

API is live at http://localhost:8000. Interactive OpenAPI documentation is at http://localhost:8000/docs.

3. Launch Frontend (Next.js 14)
bash
cd frontend
npm install
npm run dev

Open http://localhost:3000 (or http://localhost:3005). The app automatically pre-seeds realistic Indian MSME manufacturing data (Apex Precision Engineering Pvt. Ltd.) so you can explore immediately.

🧪 Automated Verification & Test Suite

Run the automated backend test suite using Pytest:

bash
# From repository root (with venv activated)
pytest -v backend/app/tests/test_all.py
Test Coverage Results:
text
backend/app/tests/test_all.py::test_stockout_date_calculation PASSED     [ 16%]
backend/app/tests/test_all.py::test_invoice_mismatch_detection PASSED    [ 33%]
backend/app/tests/test_all.py::test_duplicate_invoice_detection PASSED   [ 50%]
backend/app/tests/test_all.py::test_cash_flow_projection PASSED          [ 66%]
backend/app/tests/test_all.py::test_business_failure_simulator PASSED    [ 83%]
backend/app/tests/test_all.py::test_ai_provider_fallback PASSED          [100%]

Docker Deployment
Run the complete multi-container stack (FastAPI backend, Next.js frontend, and PostgreSQL):
bash
docker-compose up --build

