# Weather Dashboard - DevOps Assignment

![CI Pipeline](https://github.com/YOUR_USERNAME/weather-dashboard-devops/workflows/CI%20Pipeline/badge.svg)
![Deploy to Production](https://github.com/YOUR_USERNAME/weather-dashboard-devops/workflows/Deploy%20to%20Production/badge.svg)

A professional, real-time weather dashboard application built as part of the Advanced Git & DevOps Team Collaboration Assignment. Features include live weather data, 5-day forecasts, city search, and a stunning responsive UI.

## 👥 Group Information

- **Student 1:** [Full Name as in LMS] - [Student ID] - Role: DevOps/Release Manager
- **Student 2:** [Full Name as in LMS] - [Student ID] - Role: Backend Developer
- **Student 3:** [Full Name as in LMS] - [Student ID] - Role: Frontend Developer

## 📝 Project Description

Weather Dashboard is a modern, feature-rich web application that provides real-time weather information for cities worldwide. The application integrates with the OpenWeatherMap API to deliver accurate current weather conditions and 5-day forecasts. Built with a focus on user experience, it features a beautiful glassmorphic design, smooth animations, and full mobile responsiveness.

Key highlights:
- 🌍 Global city search with autocomplete
- 🌡️ Real-time weather data and 5-day forecasts
- 💾 Local storage for recent searches
- 🎨 Modern UI with glassmorphism and gradient effects
- 📱 Fully responsive design for all devices
- ⚡ Fast performance and smooth animations

## 🚀 Live Deployment

**Live URL:** [Your Netlify deployment URL will appear here]

> **Demo Mode:** The application works in demo mode with sample data by default. For live weather data, obtain a free API key from [OpenWeatherMap](https://openweathermap.org/api) and configure it in the browser console: `weatherApp.setApiKey("YOUR_API_KEY")`

## 🛠️ Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **API:** OpenWeatherMap API
- **Styling:** Modern CSS with CSS Variables, Glassmorphism, Gradients
- **Fonts:** Google Fonts (Inter)
- **CI/CD:** GitHub Actions
- **Deployment:** Netlify
- **Version Control:** Git & GitHub
- **Development Tools:** Node.js, npm

## ✨ Features

### Core Features
- **Real-time Weather Data:** Current temperature, feels like, humidity, wind speed, UV index
- **5-Day Forecast:** Daily weather predictions with icons and descriptions
- **City Search:** Smart search with autocomplete suggestions
- **Recent Searches:** Quick access to previously searched cities
- **Responsive Design:** Optimized for desktop, tablet, and mobile devices

### Technical Features
- **Demo Mode:** Works without API key using sample data
- **Error Handling:** User-friendly error messages and retry functionality
- **Local Storage:** Persistent recent searches across sessions
- **Accessibility:** Semantic HTML and ARIA labels
- **Performance:** Optimized animations and lazy loading

### UI/UX Features
- **Modern Design:** Glassmorphic cards with blur effects
- **Smooth Animations:** Fade-in, slide, and float animations
- **Dark Theme:** Eye-friendly dark color scheme
- **Visual Feedback:** Loading states, notifications, and hover effects
- **Gradient Accents:** Vibrant color gradients throughout

## 🌿 Branch Strategy

We implemented the GitFlow branching strategy:

- **`main`** - Production-ready code, protected branch, auto-deploys to Netlify
- **`develop`** - Integration branch for ongoing development
- **`feature/*`** - Feature development branches (one per team member)
  - `feature/weather-api-integration` - Weather API and backend logic
  - `feature/ui-components` - Frontend UI components and styling
  - `feature/cicd-deployment` - CI/CD pipeline and deployment setup

### Branching Workflow
1. All development starts from `develop` branch
2. Each feature is developed in its own `feature/*` branch
3. Features are merged to `develop` via Pull Requests with code reviews
4. Once `develop` is stable, it's merged to `main` for production deployment
5. `main` branch automatically triggers deployment to Netlify

## 👨‍💻 Individual Contributions

### [Student 1 Name] - DevOps/Release Manager
**Responsibilities:**
- Repository initialization and configuration
- GitHub Actions CI/CD pipeline setup
- Netlify deployment configuration
- Branch protection rules implementation
- Merge conflict resolution
- Release coordination

**Key Contributions:**
- Created `.github/workflows/ci.yml` for continuous integration
- Created `.github/workflows/deploy.yml` for automatic deployment
- Set up Netlify deployment with environment variables
- Configured branch protection for `main` branch
- Created `package.json` with build, test, and lint scripts
- Created `build.js`, `test.js`, and `lint.js` utilities
- Documented deployment process in README
- Managed pull request merges and resolved conflicts

**Commits:** [List specific commit hashes]
- `chore: initial repository setup and configuration`
- `ci: add GitHub Actions workflows for CI/CD`
- `deploy: configure Netlify deployment`
- `docs: update README with deployment instructions`

---

### [Student 2 Name] - Backend Developer
**Responsibilities:**
- Weather API integration
- Data fetching and processing
- Error handling logic
- Demo mode implementation
- Backend documentation

**Key Contributions:**
- Created `src/scripts/weather-api.js` - Complete Weather API module
- Implemented OpenWeatherMap API integration
- Built demo mode for testing without API key
- Created city search and autocomplete functionality
- Designed data formatting and validation
- Implemented error handling and retry logic
- Added support for current weather and 5-day forecast
- Documented API usage and configuration

**Commits:** [List specific commit hashes]
- `feat: implement Weather API integration`
- `feat: add demo mode with sample data`
- `feat: add city search autocomplete`
- `fix: improve error handling for API calls`

---

### [Student 3 Name] - Frontend Developer
**Responsibilities:**
- UI/UX design and implementation
- Responsive layout development
- Component styling
- User interaction handling
- README documentation

**Key Contributions:**
- Created `src/index.html` - Complete semantic HTML structure
- Created `src/styles/main.css` - Comprehensive styling system
- Created `src/scripts/ui.js` - UI management module
- Created `src/scripts/app.js` - Main application controller
- Designed glassmorphic UI with modern aesthetics
- Implemented responsive design for all devices
- Added smooth animations and transitions
- Created notification system and loading states
- Built recent searches and favorites features
- Wrote comprehensive README documentation

**Commits:** [List specific commit hashes]
- `feat: create HTML structure and layout`
- `style: implement modern CSS design system`
- `feat: add UI manager and animations`
- `feat: integrate backend with frontend`
- `docs: create comprehensive README`

## 🔧 Setup Instructions

### Prerequisites
- **Node.js** (version 18 or higher) - [Download](https://nodejs.org/)
- **Git** - [Download](https://git-scm.com/)
- **Code Editor** - VS Code, Sublime Text, or similar
- **(Optional)** OpenWeatherMap API Key - [Get Free Key](https://openweathermap.org/api)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/weather-dashboard-devops.git

# 2. Navigate to project directory
cd weather-dashboard-devops

# 3. Install dependencies
npm install

# 4. Run development server
npm run dev
```

The application will be available at `http://localhost:3000`

### Running Tests

```bash
# Run all tests
npm test

# Run linter
npm run lint

# Run build
npm run build
```

## 🚀 Deployment Process

### Automated Deployment (CI/CD)

Our project uses GitHub Actions for continuous integration and deployment:

1. **On every push/PR to `develop` or feature branches:**
   - Checkout code
   - Install dependencies
   - Run linter checks
   - Run tests
   - Build project
   - Report status

2. **On push to `main` branch:**
   - All CI checks (above)
   - Deploy to Netlify production
   - Update deployment status

### Manual Deployment to Netlify

If you want to deploy manually:

```bash
# 1. Install Netlify CLI
npm install -g netlify-cli

# 2. Login to Netlify
netlify login

# 3. Initialize Netlify site
netlify init

# 4. Deploy
netlify deploy --prod --dir=src
```

### Setting up GitHub Secrets

For automatic deployment, add these secrets to your GitHub repository:

1. Go to **Settings** → **Secrets and variables** → **Actions**
2. Add the following secrets:
   - `NETLIFY_AUTH_TOKEN` - From Netlify account settings
   - `NETLIFY_SITE_ID` - From Netlify site settings

## 📁 Project Structure

```
weather-dashboard-devops/
├── .github/
│   └── workflows/
│       ├── ci.yml              # CI pipeline workflow
│       └── deploy.yml          # Deployment workflow
├── src/
│   ├── index.html             # Main HTML file
│   ├── styles/
│   │   └── main.css           # Complete CSS styling
│   └── scripts/
│       ├── weather-api.js     # Weather API integration
│       ├── ui.js              # UI management
│       └── app.js             # Main application logic
├── .gitignore                 # Git ignore rules
├── package.json               # NPM dependencies and scripts
├── build.js                   # Build validation script
├── lint.js                    # Code linting script
├── test.js                    # Test runner script
└── README.md                  # This file
```

## 🧪 Testing

The project includes basic automated tests:

- **File Structure Validation:** Ensures all required files exist
- **Code Quality Checks:** Basic linting and style checks
- **Component Tests:** Validates HTML structure and CSS implementation

Run tests with: `npm test`

## 🤝 Collaboration Workflow

### Pull Request Process

1. Create feature branch from `develop`
2. Make changes and commit with meaningful messages
3. Push to GitHub
4. Create Pull Request to `develop`
5. Request code review from team members
6. Address review comments
7. Merge after approval

### Commit Message Convention

We follow conventional commits:

- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes (formatting)
- `refactor:` Code refactoring
- `test:` Adding tests
- `chore:` Maintenance tasks
- `ci:` CI/CD changes

Example: `feat: add 5-day weather forecast feature`

## 🐛 Challenges Faced

### Challenge 1: Merge Conflicts in CSS
**Issue:** Multiple team members edited the same CSS file, causing merge conflicts.

**Resolution:** 
- Communicated via PR comments
- Used CSS modular approach with clear sections
- Resolved conflicts by keeping both changes in separate sections
- Documented in commit: `fix: resolve merge conflicts in main.css`

### Challenge 2: API Rate Limiting
**Issue:** OpenWeatherMap free tier has API call limits.

**Resolution:**
- Implemented demo mode for testing without API calls
- Added local caching for recent searches
- Optimized API calls to reduce redundancy

### Challenge 3: CI/CD Pipeline Configuration
**Issue:** Initial GitHub Actions workflow had dependency errors.

**Resolution:**
- Updated Node.js version to 18.x
- Fixed npm scripts in package.json
- Added error handling in workflow scripts
- Used `continue-on-error` for non-critical steps

## 📚 API Documentation

### OpenWeatherMap API

To use live data instead of demo mode:

1. Sign up at [OpenWeatherMap](https://openweathermap.org/api)
2. Get your free API key
3. Open browser console on the deployed site
4. Run: `weatherApp.setApiKey("YOUR_API_KEY_HERE")`

**API Endpoints Used:**
- Current Weather: `https://api.openweathermap.org/data/2.5/weather`
- 5-Day Forecast: `https://api.openweathermap.org/data/2.5/forecast`
- City Search: `https://api.openweathermap.org/geo/1.0/direct`

## 🎯 Future Enhancements

Potential improvements for future versions:

- [ ] User accounts and saved favorite cities
- [ ] Weather alerts and notifications
- [ ] Interactive weather maps
- [ ] Historical weather data charts
- [ ] Multi-language support
- [ ] PWA (Progressive Web App) support
- [ ] Dark/Light theme toggle
- [ ] Share weather on social media

## 📄 License

This project is created for educational purposes as part of the Systems Administration & Maintenance module.

## 🙏 Acknowledgments

- **OpenWeatherMap** - For providing free weather API
- **Google Fonts** - For the Inter font family
- **Netlify** - For free hosting and deployment
- **GitHub** - For version control and CI/CD
- **Instructor:** Isuru Samarappulige - For guidance and assignment structure

---

## 📞 Contact

For any questions or issues regarding this project, please contact:
- [Student 1 Name] - [email@university.edu]
- [Student 2 Name] - [email@university.edu]
- [Student 3 Name] - [email@university.edu]

---

**Course:** Systems Administration & Maintenance  
**Assignment:** Advanced Git & DevOps Team Collaboration  
**Submission Date:** 18th January 2025  
**University:** [Your University Name]

---

<div align="center">

Made with ❤️ by the DevOps Team

![GitHub last commit](https://img.shields.io/github/last-commit/YOUR_USERNAME/weather-dashboard-devops)
![GitHub repo size](https://img.shields.io/github/repo-size/YOUR_USERNAME/weather-dashboard-devops)

</div>
