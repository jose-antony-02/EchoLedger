"# EchoLedger 💰

> **Your money, clearly.**

A modern, privacy-first personal finance application for tracking income and expenses across multiple ledgers. Built with React and designed for people who value their financial privacy.

![EchoLedger Dashboard](https://via.placeholder.com/1200x600/050810/10b981?text=EchoLedger+Dashboard)



## 🚀 Quick Start

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/jose-antony-02/EchoLedger.git
cd EchoLedger

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Build for Production

```bash
npm run build
npm run preview
```

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Framework | React 18 |
| State Management | Zustand |
| Routing | React Router v6 |
| Styling | Tailwind CSS |
| Charts | Chart.js + react-chartjs-2 |
| Storage | localStorage (offline-first) |
| Build Tool | Vite |

## 📁 Project Structure

```
echoledger/
├── src/
│   ├── components/       # Reusable UI components
│   │   ├── Dashboard.jsx
│   │   ├── TransactionItem.jsx
│   │   ├── LedgerFilter.jsx
│   │   ├── DateFilter.jsx
│   │   ├── PeriodSummaryStrip.jsx
│   │   ├── EmptyState.jsx
│   │   └── ...
│   ├── pages/            # Page components
│   │   ├── Dashboard.jsx
│   │   ├── Transactions.jsx
│   │   ├── Ledgers.jsx
│   │   ├── LedgerDetail.jsx
│   │   ├── Analytics.jsx
│   │   └── Login.jsx
│   ├── store/            # Zustand store
│   │   └── useStore.js
│   ├── utils/            # Helper functions
│   │   └── formatters.js
│   ├── App.jsx           # Main app component
│   └── main.jsx          # Entry point
├── public/               # Static assets
├── index.html
├── package.json
└── vite.config.js
```

## 🎯 Usage Guide

### Creating a Ledger

1. Navigate to **Ledgers** page
2. Click **"+ New Ledger"**
3. Enter a name (e.g., "Home Expenses", "Business", "2026 Savings")
4. Select your preferred currency
5. Click **Create**

### Adding Transactions

1. Click **"+ Add Transaction"** from any page
2. Select the ledger, type (income/expense), category
3. Enter amount and description
4. Set the date
5. Click **Save**

### Viewing Analytics

1. Navigate to **Analytics** page
2. Use the date filter to select a time period
3. View:
   - Monthly income/expense trends
   - Category-wise expense breakdown
   - Savings rate calculation
   - Period summaries (Today, Week, Month, Year, All Time)

## 🔒 Privacy & Data

- **No accounts required** — Start using immediately
- **No cloud storage** — All data stays on your device
- **No tracking** — No analytics, no cookies, no telemetry
- **No server** — Completely client-side application

### Data Location

Your data is stored in browser's `localStorage` under these keys:
- `echoledger_user` — User session
- `echoledger_ledgers` — All ledgers
- `echoledger_transactions` — All transactions
- `echoledger_categories` — Category definitions

### Backup Your Data

Since data is stored locally, consider periodic backups:

```javascript
// Open browser console and run:
const backup = {
  ledgers: localStorage.getItem('echoledger_ledgers'),
  transactions: localStorage.getItem('echoledger_transactions'),
  categories: localStorage.getItem('echoledger_categories'),
};
console.log(JSON.stringify(backup));
// Copy the output and save it securely
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow existing code style (Prettier configured)
- Write meaningful commit messages
- Test your changes thoroughly
- Update documentation if needed

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with ❤️ using React and modern web technologies
- Inspired by the need for private, offline-first finance tools
- Thanks to the open-source community for amazing libraries

## 📬 Contact

- **GitHub:** [@jose-antony-02](https://github.com/jose-antony-02)
- **Project Link:** [https://github.com/jose-antony-02/EchoLedger](https://github.com/jose-antony-02/EchoLedger)

---

<p align="center">
  <strong> EchoLedger </strong> — Private by default. Beautiful by design.
</p>

<p align="center">
  Made with 💚 for financial clarity
</p>

"
