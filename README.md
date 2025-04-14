# Product Requirements Document (PRD)

**Product Name:** Bitcoin Transaction Monitor  
**Version:** 1.0  
**Author:** Brian Groth  
**Last Updated:** April 14, 2025  
**Status:** Final Draft

---

## 1. Purpose

The Bitcoin Transaction Monitor provides real-time insights into the Bitcoin blockchain and market activities. It tracks significant transactions, mempool statistics, supply metrics, and integrates sentiment analysis with recent news headlines. It is designed for crypto enthusiasts and analysts seeking a clear, interactive dashboard.

---

## 2. Scope

This web-based, single-page static application includes:
- Largest recent Bitcoin transactions
- Mempool statistics
- Bitcoin market and supply metrics
- Fear & Greed Index displayed as a speedometer chart
- Real-time BTC price in both EUR and USD
- 24h price change with corresponding timestamp
- 7-day BTC price chart (Chart.js) labeled with title
- Latest Bitcoin news headlines via CryptoCompare API

---

## 3. Stakeholders

- **Developer:** Brian Groth  
- **End Users:** Cryptocurrency traders, investors, analysts, blockchain enthusiasts

---

## 4. Assumptions and Constraints

**Assumptions:**
- Users access the dashboard via modern browsers
- Public data APIs are accessible and responsive

**Constraints:**
- Static single-page application (no server-side logic)
- Hosted via GitHub Pages
- Uses public/free APIs (CoinGecko, Blockchain.com, Alternative.me, CryptoCompare)
- CORS handled with optional proxy selector

---

## 5. Functional Requirements

- **FR1:** Display live BTC price in both EUR and USD
- **FR2:** Visualize 24h price change with green/red indicator and reference timestamp
- **FR3:** Show market cap and 24h volume
- **FR4:** Show circulating supply and percent mined
- **FR5:** Identify and list significant transactions (>10 BTC)
- **FR6:** Classify transactions by type (Deposit, Withdrawal, Whale Transfer)
- **FR7:** Color-code transaction impact (High, Medium, Low)
- **FR8:** Present mempool size (unconfirmed transactions) with explanatory text
- **FR9:** Display Fear & Greed Index as a radial speedometer chart (1–100, red to green scale)
- **FR10:** Show latest Bitcoin news via CryptoCompare API
- **FR11:** Provide a labeled 7-day BTC price chart using Chart.js
- **FR12:** Include proxy selector to bypass CORS limitations
- **FR13:** Embed all JS and CSS within a single HTML file for static hosting

---

## 6. Non-Functional Requirements

- **NFR1:** Must run as a static site deployable via GitHub Pages
- **NFR2:** Responsive design for desktop and mobile devices
- **NFR3:** API data must refresh automatically every 60 seconds
- **NFR4:** Lightweight design with minimal dependencies
- **NFR5:** Clear labeling and explanations to guide users

---

## 7. User Interface Requirements

- Responsive layout using CSS Grid and Flexbox
- Color theme using orange, white, and light neutral backgrounds
- Card-based layout for stats, news, and transactions
- Chart.js integration for historical price display and speedometer
- Proxy dropdown menu to toggle CORS bypass services
- Badges and visual indicators for transaction types
- Footer text: "Developed by Brian Groth & ChatGPT"
- Explanation section for each stat, including Mempool Size

---

## 8. Success Metrics

- All API endpoints fetch data successfully without timeouts
- Dashboard loads in under 3 seconds
- All UI sections populated correctly on first load
- No console errors during runtime

---

## 9. Future Enhancements

- Add light/dark theme toggle
- Integrate CryptoQuant (authenticated) for deeper exchange metrics
- Add alerting system for whale transfers or spikes in mempool or volume
- Enable historical transaction tracking or export options
- Add wallet tagging support for user-added aliases

---
