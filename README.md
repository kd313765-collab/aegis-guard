# Aegis-Guard

Conflict zones ke hospitals ke liye medicine shortage early-warning system, jo dawaiyan khatam hone se pehle warning deta hai.

## Problem
War aur conflict mein hospitals ki medicine supply bigad jati hai: warehouses par attacks, road band hona, aur casualty ke baad achanak demand badhna. Maujooda systems (jaise WHO HeRAMS) mostly yeh dekhte hain ki abhi kya available hai. Aegis-Guard test karta hai ki ML model agle 7 din ka demand aur stockout risk pehle se bata sakta hai ya nahi, simple historical-average baseline se behtar.

## Features
- Agle 7 din ka medicine-wise demand forecast
- Stockout risk level (low / medium / high)
- Prediction confidence aur missing-data warnings
- Dashboard par human-reviewed alerts (approve / reject)

## Tech Stack
- Python 3.10+
- pandas, numpy, scikit-learn, xgboost
- matplotlib, streamlit
- pytest, jupyter
- (baaki libraries baad mein add karenge)

## Folder Structure
```
aegis-guard/
├── data/
│   ├── raw/          # original data (.gitkeep ke saath)
│   ├── processed/    # cleaned data
│   └── synthetic/    # generated datasets
├── docs/             # notes, diagrams, proposal
├── models/           # saved trained models
├── notebooks/        # EDA aur experiments
├── results/          # plots, tables, metrics
├── src/              # source code
├── tests/            # pytest tests
├── .gitignore
├── README.md
└── requirements.txt
```

## Setup
1. git clone <repo-url>
2. python -m venv venv
3. venv\Scripts\activate  (Mac/Linux: source venv/bin/activate)
4. pip install -r requirements.txt

## Usage
Coming soon.

## Team
- B.Tech Person : engineering (pipeline, API, dashboard)
- Pharm D Person: medicine domain expert


## Status
Month 1: Setup + tools (in progress)

Note: Abhi saare results synthetic (simulated) data par hain. Ye project clinical ya dosing decision ke liye nahi hai.
