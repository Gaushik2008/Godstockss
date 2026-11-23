# GodStocks — Website Upgrade Challenge(2026)

> **An interactive front-end concept for a clearer, more approachable stock-market learning experience.**

GodStocks is a single-page website prototype created for the **Godstockss Website Upgrade Challenge**. It explores how a stock-market platform can make market information easier to understand through a responsive interface, transparent price-status indicators, an interactive watchlist and charts, beginner-friendly explainers, and risk-free paper-trading practice.

**Project status:** Front-end demonstration. It uses generated sample market data and browser-based state. It is not connected to a broker, exchange, authentication provider, payment gateway, or production backend.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Challenge Context](#challenge-context)
- [Design Goals](#design-goals)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [How to Use the Demo](#how-to-use-the-demo)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Data, Storage, and Limitations](#data-storage-and-limitations)
- [Security and Financial Disclaimer](#security-and-financial-disclaimer)
- [Potential Next Steps](#potential-next-steps)
- [Challenge Submission](#challenge-submission)
- [Author](#author)
- [License](#license)

---

## Project Overview

Stock-market interfaces can overwhelm new users with dense tables, unfamiliar terminology, and numbers whose freshness is not always obvious. GodStocks explores a more guided experience: users can first understand the market, then inspect individual stocks, learn basic concepts, and finally practise with virtual money.

### Experience at a glance

| Area | What it offers |
|---|---|
| **Home** | Market snapshot, sample index values, market breadth, and sector heatmap |
| **Dashboard** | Personal watchlist, searchable stock list, sortable data, and interactive charts |
| **Explain** | Contextual stock explanations in English and Hindi, with a beginner-friendly glossary |
| **Alerts** | Configurable sample price alerts and in-page trigger feedback |
| **Learn and compete** | Short lessons, quizzes, a virtual wallet, practice trades, and a demo leaderboard |
| **Plans** | Illustrative Free, Pro, and Elite plan concepts with a simulated checkout flow |

Visitors can explore the core experience before creating an account.

## Challenge Context

This project was developed in response to the **Godstockss Website Upgrade Challenge**, which invites participants to identify practical improvements to the GODSTOCKSS website.

The challenge brief encourages ideas around:

- Website design, UI/UX, and responsive behaviour.
- New features and useful functionality.
- Navigation and overall user experience.
- Website performance and usability.
- Creative, practical improvements to the platform.

GodStocks turns those themes into a navigable prototype rather than a static list of suggestions. The implementation demonstrates possible user journeys across market discovery, stock research, learning, and simulated trading.

- **Challenge:** [Godstockss Website Upgrade Challenge on Unstop](https://unstop.com/quiz/godstockss-website-upgrade-challenge-godstockss-1784540)
- **Repository:** [Gaushik2008/Godstocks](https://github.com/Gaushik2008/Godstocks)

## Design Goals

1. **Make market information easier to scan.** Use clear hierarchy, restrained colour, readable numbers, and visual summaries.
2. **Make data freshness visible.** Communicate whether the interface is showing a live-style demo, delayed demo, or last-known sample value.
3. **Help beginners learn in context.** Explain common concepts beside the stock or chart being explored.
4. **Encourage practice before risk.** Provide a virtual wallet and guided lessons without using real money.
5. **Keep the experience usable across devices.** Use responsive layouts, touch-friendly controls, keyboard interactions, visible focus styles, and reduced-motion support.

---

## Features

### 1. Home and Market Overview

- Editorial-style landing section with an interactive sample market visualisation.
- Sample NIFTY 50 and SENSEX index values.
- Sample market breadth showing advancing and declining stocks.
- Sector heatmap: tile sizes represent sample weights and colours represent sample daily movement.
- Selectable heatmap tiles that open the corresponding stock chart.
- Overview of platform capabilities and illustrative subscription plans.

### 2. Market Data Status

The market-status control has three demonstration modes:

| Mode | Behaviour in this prototype |
|---|---|
| **Live** | Displays changing simulated sample values and a refresh timestamp |
| **Delayed** | Demonstrates a feed that updates on a delayed interval |
| **Offline** | Holds the last displayed values, marks them as stale, and pauses practice trading |

**Important:** These are interface states for demonstration. The project does not receive live or delayed exchange data. The labels do not represent a real market-data connection.

### 3. Personal Dashboard

- Starter watchlist available on first visit.
- Add and remove stocks.
- Search by stock symbol or company name.
- Sort by name, daily percentage change, or price.
- Select a stock to update its chart and related information.
- Personalisation flow for experience level, preferred sectors, and stocks.
- Beginner, Intermediate, and Experienced learning levels.

The prototype includes sample entries for 13 Indian-listed companies across Banking, IT, Energy, Consumer, Auto, Pharma, and Industrial & Telecom.

### 4. Charts and Stock Explainers

Each selected stock has a dedicated chart panel.

- Interactive SVG price chart.
- 1-week, 1-month, and 3-month sample ranges.
- Hover to inspect a point's date and sample price.
- Use the left and right arrow keys to inspect chart values.
- Switch between chart and tabular views.
- Display sector, sample P/E comparison, and an illustrative 52-week range.
- Open a contextual explainer from a watchlist row or chart.

The explainer includes:

- Plain-language answers about daily movement, valuation, 52-week range, and P/E.
- English and Hindi answer modes.
- Suggested questions for quick exploration.
- A glossary covering P/E, 52-week range, day change, circuit limits, and paper trading.
- Clear wording when sample data is insufficient to explain why a price moved.

Explanations are generated from values embedded in the demo. They do not use an AI service, live news, company filings, or external research sources.

### 5. Price Alerts

Users can create sample alerts by selecting:

- A stock.
- Whether the price should rise above or fall below a chosen level.
- A target price.
- One or more notification preferences: Push, Email, or WhatsApp.

The page checks configured thresholds while the demo is open, displays triggered alerts, and allows users to delete them.

**Demo limitation:** Push, email, and WhatsApp delivery are not integrated. The selected channels are stored as preferences and displayed in the in-page demonstration only.

### 6. Learning and Paper Trading

The Learn and Compete view combines introductory lessons with a simulated trading experience.

**Learning path**

1. Reading a price quote.
2. Understanding what P/E tells you.
3. Sizing a position.

Each module contains a short explanation and a multiple-choice knowledge check. Completing the first module unlocks the demo challenge-entry interaction.

**Virtual wallet**

- Starts with **₹10,00,000 in virtual cash**.
- Buy and sell sample stocks.
- Validate quantities and available virtual cash.
- View cash, holdings, total return, and open positions.
- Trading is paused when the interface is switched to Offline mode.

**Weekly Nifty Challenge**

- Join the simulated challenge after completing the first learning module.
- View a sample leaderboard.
- Track a local learning streak and achievement badges.

Leaderboard entries are illustrative, not real participants or competition results. No real order is placed and no securities are bought or sold.

### 7. Plans and Demo Checkout

The home page presents three illustrative plan concepts:

- **Free**
- **Pro**
- **Elite**

Users can switch between monthly and yearly billing views. The checkout interaction validates a demo UPI ID and simulates a successful payment response.

**No payment is processed.** The plans, prices, account state, and checkout confirmation are prototype behaviour only.

### 8. Navigation and Guided Tour

- Main navigation for Home, Dashboard, and Learn and Compete.
- Responsive bottom navigation on smaller screens.
- Hash-based navigation between views.
- Search and command palette for pages, stocks, and common actions.
- Nine-step guided tour introducing the main interactions.
- Modal dialogs for sign-in, onboarding, checkout, and stock explanations.
- Keyboard-friendly controls, visible focus states, and reduced-motion handling.

---

## Technology Stack

GodStocks is deliberately lightweight and does not require a framework or build system.

| Technology | Usage |
|---|---|
| **HTML5** | Page structure, semantic sections, forms, tables, and dialogs |
| **CSS3** | Responsive layouts, visual design, themes, transitions, and accessibility states |
| **Vanilla JavaScript** | Navigation, application state, interactions, sample data, and local persistence |
| **SVG** | Stock charts, sparklines, icons, and data visualisations |
| **HTML Canvas** | Interactive hero visualisation |
| **Browser Local Storage** | Saving demo watchlists, alerts, preferences, wallet state, and learning progress |
| **Google Fonts** | Instrument Sans, Instrument Serif, and Big Shoulders Display |

There is no framework runtime, package manager, bundler, or backend dependency.

## Project Structure

    Godstocks/
    ├── index.html                # Complete single-file website prototype
    ├── README.md                 # Project documentation
    └── GodStocks_Hackathon.pptx  # Challenge presentation

The styles, markup, and JavaScript are contained in index.html so the prototype can be opened directly in a browser.

---

## Getting Started

### Requirements

- A modern browser such as Chrome, Firefox, Edge, or Safari.
- Internet access for the Google Fonts used by the design. System font fallbacks are provided if those fonts are unavailable.

### 1. Clone the repository

    git clone https://github.com/Gaushik2008/Godstocks.git
    cd Godstocks

### 2. Open the website

No installation or build command is required.

**Option A — Open directly**

Open index.html in your browser.

**Option B — Run a local static server**

    python3 -m http.server 5500

Then visit:

    http://localhost:5500

---

## How to Use the Demo

A suggested walkthrough:

1. Open the **Home** page and inspect the market overview.
2. Switch between **Live**, **Delayed**, and **Offline** to see how the interface communicates feed status.
3. Select a sector tile in the heatmap to open a stock in the dashboard.
4. Search, sort, add, or remove stocks in the watchlist.
5. Select a stock and explore its chart using the 1W, 1M, and 3M controls.
6. Switch the chart to table view or use the **Explain** action.
7. Create a sample price alert and observe its in-page status.
8. Open **Learn and compete**, complete the lessons, and try a virtual trade.
9. Start the guided tour to see the main features in sequence.

### Demo sign-in

The authentication interface is simulated and does not create a real account.

- Email sign-in and account creation validate input locally.
- Google sign-in is a demonstration interaction only.
- Mobile OTP uses the fixed demo code:

    123456

Do not enter real passwords, personal information, or payment credentials into this prototype.

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| **Ctrl + K** | Open the search and command palette |
| **Cmd + K** | Open the search and command palette on macOS |
| **/** | Open the command palette when focus is not in a text-entry field |
| **Up / Down** | Move through command-palette results |
| **Enter** | Run the selected command |
| **Esc** | Close the active dialog or exit the guided tour |
| **Left / Right** | Inspect chart points when the chart has keyboard focus |

---

## Data, Storage, and Limitations

Understanding what is real and what is simulated is an important part of this prototype.

### Sample market data

- Stock prices, index values, historical series, P/E values, sector weights, and 52-week ranges are sample values embedded in the JavaScript.
- Historical series are generated locally for visualisation.
- A timer changes simulated values to make the interface interactive.
- No exchange feed, broker API, market-data vendor, news API, or company-filings API is connected.

### Browser storage

The prototype uses localStorage with the **gs_** key prefix to preserve selected demo state, including:

- Watchlist and experience level.
- Price alerts.
- Virtual wallet and positions.
- Learning progress and challenge participation state.
- Selected plan and learning streak.

This information is stored in the browser profile on the device where the demo is used. It is not synchronised to a server. Clearing browser site data may reset the saved demo state.

### Integrations not implemented

| Capability shown in the interface | Current prototype status |
|---|---|
| Live market data | Simulated only |
| Delayed market data | Simulated only |
| User authentication | Local demonstration only |
| Google sign-in | Simulated only |
| Mobile OTP | Fixed demo OTP |
| Email verification and password reset | Simulated only |
| Push, email, and WhatsApp alerts | In-page demonstration only |
| UPI payment | Simulated only |
| AI-powered explanations | Rule-based sample-data explanations |
| News and company filings | Not connected |
| Real broker orders | Not implemented |
| Server-side database | Not implemented |

---

## Security and Financial Disclaimer

GodStocks is an educational UI/UX prototype, not a financial product.

- All market values are sample data and must not be treated as live quotes.
- The project does not provide investment recommendations or financial advice.
- Paper trades use virtual money and do not reach a broker or exchange.
- No real payment is collected.
- Authentication and OTP flows are not secure production authentication.
- Do not submit real credentials, personal information, or financial details.

Always verify market information through an authorised financial-data provider or broker before making an investment decision.

## Potential Next Steps

The following are possible future development directions, not features currently available in this repository.

- Connect a licensed market-data provider and display source, exchange timestamp, and data-delay information.
- Introduce a backend API and database for user accounts, watchlists, alerts, and learning progress.
- Replace demo authentication with a secure identity provider, server-side sessions, and verified OTP delivery.
- Connect alert delivery to real notification services with user consent and delivery-status tracking.
- Add a genuine paper-trading engine with transaction history, portfolio valuation, and transparent evaluation rules.
- Integrate sourced company announcements and news with links and publication timestamps.
- Add automated tests, performance checks, and a deployment workflow.
- Conduct usability testing with beginner and experienced users.

Any production integration involving financial data, trading, identity, or payments would require appropriate security, licensing, compliance, and operational review.

---

## Challenge Submission

This repository contains the working front-end demonstration and the accompanying presentation.

- **Unstop challenge page:** [Godstockss Website Upgrade Challenge](https://unstop.com/quiz/godstockss-website-upgrade-challenge-godstockss-1784540)
- **Source code:** [GitHub repository](https://github.com/Gaushik2008/Godstocks)
- **Presentation:** [GodStocks_Hackathon.pptx](./GodStocks_Hackathon.pptx)

## Author

**Gaushik Kumar G**

GitHub: [@Gaushik2008](https://github.com/Gaushik2008)

## License

No license file is currently included in this repository. Unless a license is added, the source code is not automatically granted an open-source reuse license. Please contact the repository owner for permission before redistributing or reusing the project.
