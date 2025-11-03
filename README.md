# BoreDM - Boring/Drilling Management PDF Generator

A React-based web application that generates professional PDF documents for geological boring and drilling reports. This project creates standardized, formatted drilling documentation for construction and geological projects.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Development](#development)
- [Build](#build)
- [Contributing](#contributing)

---

## Overview

**BoreDM** is designed to streamline the creation of drilling report documentation. Instead of manually filling out paper forms or Word documents, this application generates professional PDF reports with a single click, directly in the browser.

The application currently generates reports for the **Riverside Condominiums - General Location Project** and can be customized for various drilling projects.

---

## Features

- **Client-Side PDF Generation** - No server required, all processing happens in the browser
- **Professional Formatting** - A4-sized documents with standardized layout
- **Instant Download** - One-click PDF generation and download
- **React-Based** - Modern component architecture for maintainability
- **Responsive Design** - Works on desktop and mobile browsers
- **Customizable Templates** - Easy to modify report structure and styling

---

## Technology Stack

### Core Technologies
- **React 19.0.0** - UI framework for component-based architecture
- **React DOM 19.0.0** - React rendering for web browsers
- **@react-pdf/renderer 4.3.0** - PDF document generation from React components

### Build Tools
- **react-scripts 5.0.0** - Create React App toolchain (Webpack, Babel, etc.)
- **TypeScript 5.7.2** - Type definitions for enhanced development experience

### Development Dependencies
- **ajv 8.17.1** - JSON schema validator
- **loader-utils 3.2.1** - Webpack loader utilities

---

## Project Structure

```
BoreDM/
├── public/
│   └── index.html              # HTML entry point
├── src/
│   ├── index.js                # React root entry point (13 lines)
│   ├── App.js                  # Main application component (139 lines)
│   ├── styles.js               # PDF styling definitions (135 lines)
│   └── styles.css              # Global web page styles (4 lines)
├── .gitignore                  # Git ignore rules
├── package.json                # Project dependencies and scripts
├── package-lock.json           # Locked dependency versions
└── README.md                   # Project documentation (this file)
```

---

## Getting Started

### Prerequisites

- **Node.js** (version 14.x or higher recommended)
- **npm** (comes with Node.js)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd BoreDM
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   - Navigate to [http://localhost:3000](http://localhost:3000)
   - The app will automatically reload when you make changes

---

## Usage

### Generating a PDF Report

1. Launch the application in your browser
2. Click the **"Download PDF"** button
3. The PDF will be generated and automatically downloaded as `Result.pdf`
4. Open the PDF to view your formatted drilling report

### Customizing the Report

To modify the report content:

1. **Edit data in [src/App.js](src/App.js)**
   - Locate the `MyDoc` component
   - Update text values within the `<Text>` components

2. **Modify styling in [src/styles.js](src/styles.js)**
   - Adjust font sizes, padding, colors, borders
   - Uses flexbox-based layout system

3. **Change page layout**
   - Modify `<Page>` component properties in App.js
   - Supported sizes: A4, Letter, Legal, etc.

---

## Development

### Available Scripts

#### `npm start`
Runs the app in development mode.
- Opens [http://localhost:3000](http://localhost:3000) in your browser
- Hot-reloads on file changes
- Shows lint errors in the console

#### `npm test`
Launches the test runner in interactive watch mode.
- Uses Jest testing framework
- Includes jsdom environment for DOM testing

#### `npm run build`
Builds the app for production to the `build` folder.
- Optimizes the build for best performance
- Bundles React in production mode
- Minifies code and generates source maps
- Files are hashed for cache busting

#### `npm run eject`
**Note: This is a one-way operation. Once you eject, you can't go back!**

Ejects from Create React App, giving you full control over:
- Webpack configuration
- Babel configuration
- ESLint configuration
- Build scripts

---

## Build

To create a production-ready build:

```bash
npm run build
```

This will:
1. Create an optimized production build in the `build/` folder
2. Minify JavaScript and CSS
3. Hash filenames for caching
4. Generate source maps for debugging

### Deploying

The `build` folder can be deployed to any static hosting service:
- **GitHub Pages**
- **Netlify**
- **Vercel**
- **AWS S3 + CloudFront**
- **Firebase Hosting**

---

## Browser Support

This project supports browsers with the following criteria:
- `>0.2%` market share
- Not dead browsers
- Not IE 11 or older

Specific targets:
- **Production**: Modern browsers (last 2 versions)
- **Development**: Latest Chrome, Firefox, Safari

---

## Contributing

### Development Workflow

1. Create a feature branch
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes and commit
   ```bash
   git add .
   git commit -m "Add: your feature description"
   ```

3. Push to the repository
   ```bash
   git push origin feature/your-feature-name
   ```

4. Create a Pull Request

### Coding Standards

- Use meaningful variable and function names
- Write clean, self-documenting code
- Add comments for complex logic
- Keep components small and focused
- Follow React best practices and hooks guidelines

---

## Project History

Recent commits:
- **47a5d8d** - Remove unnecessary comments from index.html for cleaner code
- **6146219** - Update dependencies and modify text style in App component
- **921eabd** - Update styles for PDF generation: adjust padding and font sizes for better layout
- **f0e6fec** - Initialize React project with essential files and PDF generation functionality
- **6e0a660** - First commit

---

## License

This project is private and part of a BoreDM assessment.

---

## Contact & Support

For questions or issues, please contact the project maintainer or open an issue in the repository.

---

## Acknowledgments

- Built with [Create React App](https://create-react-app.dev/)
- PDF generation powered by [@react-pdf/renderer](https://react-pdf.org/)
- React framework by [Meta/Facebook](https://react.dev/)

---

**Last Updated**: November 2025
