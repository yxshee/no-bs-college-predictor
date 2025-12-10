# Changelog

All notable changes to the **No-BS College Predictor** project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Planned
- Add search functionality for institutes
- Add bookmark/save predictions feature
- Add comparison view for colleges
- PWA offline support

---

## [2.0.0] - 2026-01-29

### 🎨 Major UI Overhaul

Complete redesign with a minimalist, premium black and white theme.

### Added
- Premium dark theme with CSS variables for consistent theming
- Improved responsive design for all screen sizes
- Better visual hierarchy in prediction tables
- Enhanced form styling with modern inputs

### Changed
- **BREAKING:** Upgraded from React 16.13.1 to React 18.2.0
- Updated to use `createRoot` API (React 18)
- Refactored all components to use modern React patterns
- Improved code organization and cleanup

### Fixed
- Fixed React compatibility issues with Webpack 5
- Resolved "Objects are not valid as React child" error
- Fixed ESLint configuration for CI/CD builds
- Improved table column alignment

### Security
- No personal data collection (unchanged)
- All processing happens client-side

---

## [1.0.0] - 2024-XX-XX

### 🚀 Initial Release

The first public release of No-BS College Predictor.

### Added
- JEE Mains and Advanced college predictions
- Category-based filtering (OPEN, OBC, SC, ST, EWS, PwD)
- Quota filtering (AI, HS, OS, etc.)
- Seat type filtering (Gender-Neutral, Female-Only)
- Course duration filtering (4 Years, 5 Years)
- Responsive design for mobile and desktop
- Based on JoSAA Round 7 closing ranks data

### Features
- Instant predictions without login
- Zero data collection
- Clean, simple interface
- No advertisements

---

## Version History Summary

| Version | Date | Highlights |
|---------|------|------------|
| 2.0.0 | 2026-01-29 | React 18 upgrade, dark theme, major UI overhaul |
| 1.0.0 | 2024-XX-XX | Initial release with core prediction features |

---

## Migration Guide

### Upgrading from 1.x to 2.x

If you're running a local version of 1.x, here's how to upgrade:

```bash
# 1. Pull the latest changes
git pull origin main

# 2. Remove old dependencies
rm -rf node_modules package-lock.json

# 3. Install new dependencies
npm install

# 4. Start the app
npm start
```

**Breaking Changes:**
- React 18 is now required
- The app now uses `createRoot` instead of `ReactDOM.render`
- CSS has been completely rewritten with CSS variables

---

## How to Read This Changelog

- **Added** for new features
- **Changed** for changes in existing functionality
- **Deprecated** for soon-to-be removed features
- **Removed** for now removed features
- **Fixed** for any bug fixes
- **Security** for vulnerability fixes

---

<div align="center">

📝 **Keep track of what's new!**

[View all releases on GitHub](https://github.com/yxshee/no-bs-college-predictor/releases)

</div>
