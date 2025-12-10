<div align="center">

# 🎓 No-BS College Predictor

### *Because your future shouldn't require a login.*

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-no--bs--predictor.netlify.app-00C7B7?style=for-the-badge&logo=netlify)](https://no-bs-predictor.netlify.app/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![React](https://img.shields.io/badge/React-18.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](CONTRIBUTING.md)

<br />

**A minimalist, privacy-first JEE college prediction tool that respects your time and data.**

*No signups. No ads. No BS.*

<br />

[View Demo](https://no-bs-predictor.netlify.app/) · [Report Bug](https://github.com/yxshee/no-bs-college-predictor/issues) · [Request Feature](https://github.com/yxshee/no-bs-college-predictor/issues)

</div>

---

## ✨ Why This Exists

Every year, millions of students take JEE exams in India. After results, they're bombarded with:
- 📝 Websites requiring registration just to see predictions
- 📧 Spam emails and calls from coaching centers
- 💰 "Premium" predictions behind paywalls
- 🍪 Cookies tracking every move

**No-BS College Predictor** cuts through all that noise. Enter your rank, get predictions. That's it.

---

## 🎯 Features

<table>
<tr>
<td width="50%">

### ⚡ Instant Results
Get college predictions in under 2 seconds. No loading screens, no "processing your request."

### 🔒 Zero Data Collection
We don't want your email, phone number, or "career preferences." Your rank stays in your browser.

### 📱 Responsive Design
Works flawlessly on desktop, tablet, and mobile. Predict colleges from anywhere.

</td>
<td width="50%">

### 🎨 Clean Interface
Premium black & white theme. No clutter, no distractions, no banner ads.

### 📊 Comprehensive Filtering
Filter by category (OPEN, OBC, SC, ST, EWS, PwD), quota, seat type, and course duration.

### 🏫 Both JEE Exams
Supports predictions for both JEE Mains (NITs, IIITs) and JEE Advanced (IITs).

</td>
</tr>
</table>

---

## 🚀 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yxshee/no-bs-college-predictor.git

# Navigate to project directory
cd no-bs-college-predictor

# Install dependencies
npm install

# Start development server
npm start
```

The app will open at [http://localhost:3000](http://localhost:3000) 🎉

### Production Build

```bash
# Create optimized production build
npm run build

# The build folder is ready to be deployed
```

---

## 🏗️ Project Structure

```
no-bs-college-predictor/
├── 📁 public/
│   ├── index.html          # HTML template
│   ├── manifest.json       # PWA manifest
│   └── robots.txt          # SEO config
├── 📁 src/
│   ├── 📁 components/
│   │   ├── 📁 CollegePredictor/    # Main predictor form
│   │   ├── 📁 PredictionTable/     # Results table display
│   │   └── 📁 TableFilter/         # Filter dropdowns
│   ├── 📁 utils/
│   │   ├── constants.js            # App constants & columns
│   │   ├── getData.js              # Data fetching logic
│   │   └── 📁 dataSources/
│   │       └── categoricalData.json # College data by category
│   ├── App.js              # Root component
│   ├── App.css             # Global styles
│   ├── index.js            # Entry point (React 18)
│   └── index.css           # CSS variables & theme
├── 📁 data-scripts/        # Data processing utilities
├── package.json
├── LICENSE
└── README.md
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **React 18** | UI framework with modern hooks & concurrent features |
| **CSS Variables** | Dynamic theming and consistent styling |
| **Create React App 5** | Zero-config build tooling |
| **Netlify** | Continuous deployment & global CDN |

---

## 📊 Data Source

Predictions are based on **JoSAA (Joint Seat Allocation Authority) Round 7 closing ranks** from previous counseling sessions. This data represents the final cutoffs after all rounds of seat allocation, providing the most accurate predictions possible.

### Supported Categories

| Category | Description |
|----------|-------------|
| OPEN | General category (unreserved) |
| OPEN (PwD) | General + Person with Disability |
| GEN-EWS | Economically Weaker Section |
| GEN-EWS (PwD) | EWS + Person with Disability |
| OBC-NCL | Other Backward Classes - Non-Creamy Layer |
| OBC-NCL (PwD) | OBC + Person with Disability |
| SC | Scheduled Caste |
| SC (PwD) | SC + Person with Disability |
| ST | Scheduled Tribe |
| ST (PwD) | ST + Person with Disability |

### Supported Quotas

- **AI** - All India
- **HS** - Home State
- **OS** - Other State
- **AP** - Andhra Pradesh
- **GO** - Goa

---

## 🎨 Design Philosophy

This project follows a **"less is more"** approach:

```
┌─────────────────────────────────────────────────────────┐
│                                                         │
│   ■ Monochrome palette    → Reduced eye strain          │
│   ■ Minimal interactions  → Every click is meaningful   │
│   ■ No flashy animations  → Function over form          │
│   ■ High contrast         → Accessibility first         │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

**Color Palette:**
- Background: `#0a0a0a` (near black)
- Primary Text: `#ffffff` (white)
- Accent: `#ffffff` (white)
- Borders: `#333333` (dark gray)
- Muted Text: `#888888` (medium gray)

---

## 🤝 Contributing

Contributions make the open-source community amazing! Any contributions you make are **greatly appreciated**.

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

### Quick Contribution Steps

```bash
# 1. Fork the Project (click Fork button on GitHub)

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/no-bs-college-predictor.git

# 3. Create your Feature Branch
git checkout -b feature/AmazingFeature

# 4. Make your changes and commit
git commit -m 'Add some AmazingFeature'

# 5. Push to the Branch
git push origin feature/AmazingFeature

# 6. Open a Pull Request on GitHub
```

### Ideas for Contributions

- 🆕 Add data for newer JoSAA rounds
- 🎨 Improve UI/UX
- 📱 Enhanced mobile experience
- 🔍 Add search functionality
- 📈 Add analytics for popular choices
- 🌐 Internationalization (i18n)

---

## 📜 License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for more information.

```
MIT License - Do whatever you want, just don't blame me if it breaks.
```

---

## 📋 Changelog

See [CHANGELOG.md](CHANGELOG.md) for a detailed version history.

---

## 🙏 Acknowledgments

- **JoSAA** for making counseling data publicly available
- **All JEE aspirants** who deserve better tools
- **The React community** for excellent documentation
- Coffee ☕ for making late-night coding possible

---

## 📬 Contact

**yxshee** - [@yxshee](https://github.com/yxshee)

🔗 **Project Link:** [github.com/yxshee/no-bs-college-predictor](https://github.com/yxshee/no-bs-college-predictor)

🌐 **Live Demo:** [no-bs-predictor.netlify.app](https://no-bs-predictor.netlify.app/)

---

<div align="center">

### ⭐ Star this repo if it helped you!

**Made with 🖤 for JEE aspirants everywhere**

<br />

```
 _   _           ____   ____  
| \ | | ___     | __ ) / ___| 
|  \| |/ _ \ __ |  _ \ \___ \ 
| |\  | (_) |__|| |_) | ___) |
|_| \_|\___/    |____/ |____/ 
                              
   College Predictor
```

</div>
