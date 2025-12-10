# Contributing to No-BS College Predictor

First off, thanks for taking the time to contribute! 🎉

The following is a set of guidelines for contributing to No-BS College Predictor. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [How Can I Contribute?](#how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
  - [Pull Requests](#pull-requests)
- [Style Guides](#style-guides)
  - [Git Commit Messages](#git-commit-messages)
  - [JavaScript Style Guide](#javascript-style-guide)
  - [CSS Style Guide](#css-style-guide)
- [Project Structure](#project-structure)

---

## Code of Conduct

This project and everyone participating in it is governed by our commitment to creating a welcoming environment. By participating, you are expected to uphold this standard. Please be respectful and constructive in all interactions.

**Our Standards:**
- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

---

## I Have a Question

> **Note:** If you want to ask a question, please make sure you have:
> 1. Read the [README](README.md)
> 2. Searched for existing [Issues](https://github.com/yxshee/no-bs-college-predictor/issues) that might answer your question

If you still have questions:
- Open an [Issue](https://github.com/yxshee/no-bs-college-predictor/issues/new) with the label `question`
- Provide as much context as possible
- Include relevant project and platform versions

---

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues as you might find that you don't need to create one. When you are creating a bug report, please include as many details as possible.

**How Do I Submit a Good Bug Report?**

Bugs are tracked as [GitHub issues](https://github.com/yxshee/no-bs-college-predictor/issues). Create an issue and provide the following information:

```markdown
**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Environment:**
 - OS: [e.g. macOS, Windows, Linux]
 - Browser: [e.g. Chrome 120, Firefox 121, Safari 17]
 - Node.js version: [e.g. 18.19.0]

**Additional context**
Add any other context about the problem here.
```

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

- **A clear and descriptive title**
- **A detailed description** of the suggested enhancement
- **The motivation** - why would this be useful?
- **Possible implementation** - if you have ideas on how to implement it

**Great Enhancement Ideas:**
- 📊 New filtering options
- 🎨 UI/UX improvements
- 📱 Mobile experience enhancements
- 🔍 Search functionality
- 📈 Data visualization features
- 🌐 Accessibility improvements

### Your First Code Contribution

Unsure where to begin? You can start by looking through these issues:

- **`good first issue`** - issues which should only require a few lines of code
- **`help wanted`** - issues which need extra attention
- **`documentation`** - help improve our docs

**Local Development Setup:**

```bash
# 1. Fork the repository on GitHub

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/no-bs-college-predictor.git
cd no-bs-college-predictor

# 3. Add upstream remote
git remote add upstream https://github.com/yxshee/no-bs-college-predictor.git

# 4. Install dependencies
npm install

# 5. Create a branch for your changes
git checkout -b feature/your-feature-name

# 6. Start the development server
npm start

# 7. Make your changes and test them locally

# 8. Commit your changes
git add .
git commit -m "feat: add your feature description"

# 9. Push to your fork
git push origin feature/your-feature-name

# 10. Create a Pull Request on GitHub
```

### Pull Requests

Please follow these steps to have your contribution considered:

1. **Follow the [style guides](#style-guides)**
2. **Update documentation** if you're changing functionality
3. **Add tests** if applicable
4. **Ensure the test suite passes** (`npm test`)
5. **Make sure your code lints** (`npm run lint`)
6. **Write a clear PR description** explaining what and why

**PR Title Format:**
```
type(scope): description

Examples:
feat(filters): add course duration filter
fix(table): correct column alignment on mobile
docs(readme): update installation instructions
style(css): improve button hover states
refactor(utils): simplify data fetching logic
```

---

## Style Guides

### Git Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

**Types:**
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that don't affect code meaning (formatting, etc.)
- `refactor`: Code change that neither fixes a bug nor adds a feature
- `perf`: Performance improvement
- `test`: Adding or correcting tests
- `chore`: Changes to build process or auxiliary tools

**Examples:**
```bash
feat(predictor): add support for JEE Advanced predictions
fix(table): resolve sorting issue with closing ranks
docs(readme): add contributing guidelines
style(css): update color variables for dark theme
refactor(getData): simplify category data fetching
```

### JavaScript Style Guide

- Use **ES6+** features (arrow functions, destructuring, etc.)
- Use **functional components** with hooks (no class components)
- Use **meaningful variable and function names**
- Add comments for complex logic
- Prefer **const** over let, avoid var

```javascript
// ✅ Good
const filterColleges = (colleges, rank) => {
  return colleges.filter((college) => rank <= college.closingRank)
}

// ❌ Bad
function filter(c, r) {
  var result = []
  for (var i = 0; i < c.length; i++) {
    if (r <= c[i].closingRank) result.push(c[i])
  }
  return result
}
```

### CSS Style Guide

- Use **CSS Variables** for theming
- Follow **BEM naming convention** where applicable
- Keep specificity low
- Mobile-first responsive design

```css
/* ✅ Good */
.filter-form {
  background: var(--bg-card);
  padding: var(--spacing-md);
}

.filter-form__input {
  border: 1px solid var(--border);
}

/* ❌ Bad */
div.filterForm {
  background: #1a1a1a;
  padding: 20px;
}
```

---

## Project Structure

Understanding the project structure will help you contribute effectively:

```
src/
├── components/
│   ├── CollegePredictor/      # Main form component
│   │   ├── CollegePredictor.js
│   │   └── CollegePredictor.css
│   ├── PredictionTable/       # Results table
│   │   ├── PredictionTable.js
│   │   └── PredictionTable.css
│   └── TableFilter/           # Filter dropdowns
│       ├── TableFilter.js
│       └── TableFilter.css
├── utils/
│   ├── constants.js           # App-wide constants
│   ├── getData.js             # Data fetching utilities
│   └── dataSources/
│       └── categoricalData.json  # College data
├── App.js                     # Root component
├── App.css                    # App-level styles
├── index.js                   # Entry point
└── index.css                  # Global styles & CSS variables
```

**Key Files:**
- `src/utils/constants.js` - Categories, quotas, columns configuration
- `src/utils/dataSources/categoricalData.json` - All college data by category
- `src/index.css` - Theme variables and global styles

---

## Thank You! 🙏

Your contributions to open source, large or small, make great projects like this possible. Thank you for taking the time to contribute.

---

<div align="center">

**Happy Contributing!** 🎉

</div>
