# Braam Kotze — Automation Developer Portfolio

> Python automation, web scraping, API integrations, and AI agent workflows.

## About

Civil engineer turned automation developer. I build production systems that save time and generate revenue — not tutorials, not proof-of-concepts. Real deployments, real users, real money.

- 🛒 **Shop Guru** — multi-store grocery price comparison PWA (16,000+ products, 7 retailers)
- 📈 **CFD Trading Agent** — automated trading system (9 instruments, 160+ trades, +6% returns)
- 🤖 **AI Agent (Schmarag)** — 24/7 autonomous operations manager (cron jobs, security, data pipelines)

## Skills

- **Python** — automation, scraping, trading systems, API integrations
- **Web Scraping** — Playwright, Selenium, REST APIs, GTM dataLayer, anti-bot handling
- **API Integration** — REST, GraphQL, Magento, Hybris, IG Markets, Telegram Bot API
- **AI/LLM** — OpenAI, Anthropic, local models (Ollama), multi-step agent workflows
- **Full-stack** — Node.js/Express, React/Vite, SQLite, PWA, Render deployment
- **DevOps** — cron scheduling, git pipelines, auto-deploy, security auditing

## Contact

- **Upwork:** [braam-kotze](https://www.upwork.com/freelancers/~0135ec63e8cedeed48)
- **GitHub:** [ASKotze](https://github.com/ASKotze)
- **Live Demo:** [shopguru.schmarag.com](https://shopguru.schmarag.com)

---

## Project 1: Shop Guru 🛒

**Live site:** [shopguru.schmarag.com](https://shopguru.schmarag.com)

A Progressive Web App that compares grocery prices across 7 South African retailers. Scrapes 16,000+ products, matches equivalent items across stores, and optimizes your shopping list for lowest total cost including delivery fees.

### What it does
- Scrapes prices from Checkers, Pick n Pay, Woolworths, Spar, Shoprite, Clicks, and Dis-Chem
- Matches equivalent products across stores (15,984 product groups)
- Optimizes shopping lists — auto-allocates items to cheapest store
- Tracks loyalty pricing (XtraSavings, WRP, Benefit, ClubCard)
- Delivery vs in-store modes with fee calculations
- Budget tracking (monthly + weekly)
- Price alerts with push notifications
- Price trend history per product
- Works offline (PWA), installable on mobile
- Covers 218 cities across all 9 SA provinces

### Tech stack
- **Backend:** Node.js, Express, SQLite
- **Frontend:** React, Vite, Zustand, PWA (service worker, manifest)
- **Scraping:** Playwright (browser automation), REST APIs (headless)
- **Deploy:** Render (auto-deploys on git push), seed data recovery

### Stats
- 16,754 products in database
- 17,713 current prices
- 7 shops, 218 cities, 9 provinces
- Scrapers run in 3 batches (~20 min total)
- PWA v26

---

## Project 2: CFD Trading Agent 📈

An automated CFD trading system that scans 9 financial instruments 3 times per day, generates signals using technical indicators, and executes trades on IG Markets with full risk management.

### What it does
- Scans forex (EURUSD, GBPUSD, USDJPY), indices (US500, USTECH100, DAX40, FTSE100, HK_HSI50), and commodities (GOLD, OIL_WTI)
- Two strategies: EMA_CROSS (forex/gold) and TREND_BREAK (indices/oil)
- Position sizing: 1% risk per trade, 2:1 reward:risk ratio
- ATR-based stop-loss, correlation guard, cooldown system
- Friday close-out (all positions closed before weekend)
- Results delivered via Telegram

### Strategies
- **EMA_CROSS:** Fast/slow EMA crossover + ADX>25 + RSI filter + Bollinger Bands
- **TREND_BREAK:** Donchian 20-period breakout + ADX>30 + DI confirmation + RSI filter

### Tech stack
- **Python 3.12** with virtualenv
- **yfinance** — free market data (no broker data allowance consumed)
- **IG Markets API** — trade execution only
- **pandas / numpy** — technical analysis
- **Cron (OpenClaw)** — scheduled scans

### Results
- Starting balance: $18,493.95 (demo)
- Current balance: ~$19,603 (+6%)
- 160 completed trades
- Forex + Gold: 70% win rate
- Strategy iteration improved overall win rate from 36% → 67% over 4 weeks

---

## Project 3: AI Agent — Schmarag 🤖

A 24/7 autonomous AI agent running on a Linux server that manages trading systems, web scraping, security audits, and project coordination.

### What it does
- Runs 11 automated cron jobs (trading scans, scrapers, security audits, backups, lottery analysis)
- Manages the CFD trading agent (scans, Friday close, maintenance reports)
- Manages Shop Guru scraping pipeline and auto-deployment
- Performs daily security audits (SSH, firewall, disk encryption, updates)
- Runs lottery number analysis (statistical models, not random)
- Coordinates multiple projects with progress tracking
- Communicates via Telegram and webchat

### Tech stack
- **OpenClaw** — AI agent framework (Node.js)
- **Python** — trading, scraping, analysis
- **Cron** — scheduled task execution
- **Telegram Bot API** — notifications and user interaction
- **LLM integration** — cloud and local models

### Automation schedule
| Job | Schedule | Description |
|-----|----------|-------------|
| Trading scans | 3x/day weekdays | Market analysis + trade execution |
| Friday close | Fri 17:00 | Close all positions before weekend |
| Trading maintenance | Mon/Wed/Fri 17:00 | Performance reports |
| Shop Guru scrape | Mon–Thu 20:00 | Price scraping + auto-deploy |
| Security audit | Daily 15:00 | System hardening checks |
| GitHub backup | Daily 15:30 | Automated repository backups |
| Lottery picks | 4x/week | Calculated number analysis |

---

## Background

- **BEng Civil Engineering** (Rand Afrikaans University / University of Johannesburg, 1999)
- 10 years construction project management (2000–2010)
- 9 years construction plant hire company owner (2010–2019)
- Transitioned to software development and automation (2019–present)

Engineering discipline applied to software: structured approach, risk management, production-grade delivery.

---

*All projects are real, production systems — not tutorials or demos. Code available on request for prospective clients.*