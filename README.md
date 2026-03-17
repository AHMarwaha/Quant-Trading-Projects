# Quant Trading Projects: Market Microstructure + Statistical Arbitrage

This repository contains two end-to-end quantitative trading projects designed to demonstrate the core skills expected in research and trading interviews at top firms. Together, the projects cover market microstructure, event-driven simulation, inventory-aware market making, statistical arbitrage, walk-forward validation, transaction-cost modeling, and reproducible quantitative research workflows.

## Projects Included

### 1. Limit Order Book Microstructure Simulator
A Python-based market microstructure project that simulates a stylized electronic market with stochastic order flow, adverse selection, and latency-aware market making. The strategy posts bid/ask quotes around a reservation price, dynamically adjusts spreads based on volatility and toxic flow, and manages inventory risk over time.

**Key concepts covered**
- limit order book dynamics
- event-driven simulation
- order flow imbalance
- adverse selection
- inventory-aware quoting
- spread capture
- latency and slippage modeling
- mark-to-market PnL analysis

**Core deliverables**
- limit order book simulation engine
- inventory-aware market-making strategy
- fill-probability and toxicity model
- performance analytics and diagnostics
- saved timeseries, plots, and metrics

---

### 2. Statistical Arbitrage Research Pipeline
A fully reproducible stat-arb research project that constructs a synthetic multi-asset universe, identifies mean-reverting relationships, generates spread-based trading signals, and evaluates strategy performance through a walk-forward backtesting framework. The project explicitly includes trading frictions and cost-aware performance measurement.

**Key concepts covered**
- statistical arbitrage
- pair selection
- residual/spread modeling
- z-score signal generation
- walk-forward validation
- turnover-aware transaction costs
- performance attribution
- risk-adjusted evaluation

**Core deliverables**
- synthetic multi-asset data generator
- pair selection framework
- feature engineering and signal engine
- walk-forward backtesting engine
- transaction-cost model
- portfolio and performance diagnostics

---

## Repository Goals

These projects were built to be:

- **self-contained**: no external data required
- **reproducible**: deterministic runs with fixed random seeds
- **transparent**: assumptions and modeling choices are explicit
- **interview-friendly**: easy to explain, extend, and defend
- **research-oriented**: structured like quantitative strategy prototypes rather than toy examples

The code is intentionally designed to show both **technical implementation ability** and **quantitative reasoning**.

## Reproducibility

Both projects are deterministic under fixed seeds and produce the same outputs on repeated runs, subject to the same Python and dependency versions.

Each project:
- sets a fixed NumPy random seed
- generates synthetic data internally
- saves outputs to local folders
- produces plots, CSV files, and JSON metrics
- avoids hidden dependencies on external APIs or data vendors

## Output Artifacts

Running the projects generates artifacts such as:

- simulation or backtest timeseries
- summary performance metrics
- equity / PnL curves
- inventory and position diagnostics
- spread / signal plots
- cost and adverse-selection diagnostics
- JSON summaries for easy inspection
