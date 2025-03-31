# Feel Timer Landing Page

A modern, responsive landing page for the Feel Timer app, deployed with Firebase Hosting.

## Project Overview

This repository contains the landing page for Feel Timer, an app that helps users track their time with emotional context. The landing page is built with HTML, CSS, and JavaScript, and is hosted on Firebase Hosting.

## Live Demo

The live version of the landing page can be accessed at: [https://feel-timer-app.web.app](https://feel-timer-app.web.app)

## Project Structure

```
feelTimerLP/
├── public/             # Public directory (deployed to Firebase Hosting)
│   ├── index.html      # Main landing page
│   └── 404.html        # 404 error page
├── firebase.json       # Firebase configuration
├── .firebaserc         # Firebase project association
└── README.md           # Project documentation
```

## Setup and Deployment Instructions

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or later recommended)
- [Firebase CLI](https://firebase.google.com/docs/cli) (install with `npm install -g firebase-tools`)

### Initial Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/feelTimerLP.git
   cd feelTimerLP
   ```

2. Log in to Firebase:
   ```bash
   firebase login
   ```

3. Initialize Firebase in the project directory (if not already done):
   ```bash
   firebase init hosting
   ```
   - Select the Firebase project (feel-timer-app)
   - Set the public directory to `public`
   - Configure as a single-page app: No
   - Set up automatic builds and deploys with GitHub: No

### Making Changes

1. Edit the files in the `public` directory as needed.
2. Test your changes locally:
   ```bash
   firebase serve
   ```
   This will start a local development server, typically at http://localhost:5000

### Deployment

To deploy the landing page to Firebase Hosting:

```bash
firebase deploy --only hosting
```

After successful deployment, the site will be available at:
- https://feel-timer-app.web.app
- https://feel-timer-app.firebaseapp.com

## Development Guidelines

### HTML Structure

The landing page is structured with semantic HTML5 elements:
- `<header>` for the navigation bar
- `<section>` elements for different content areas
- `<footer>` for the site footer

### CSS Styling

The styling is done with vanilla CSS using:
- Flexbox and Grid for layout
- Media queries for responsiveness
- CSS variables for consistent theming

### Best Practices

When making changes to the landing page:
1. Maintain responsive design for all screen sizes
2. Optimize images before adding them
3. Keep the code clean and well-commented
4. Test on multiple browsers before deployment

## Troubleshooting

### Common Issues

1. **"Not in a Firebase app directory" error**:
   - Make sure you have `firebase.json` in your project root
   - Run `firebase init hosting` to set up Firebase

2. **Deployment fails**:
   - Check if you're logged in with `firebase login`
   - Verify you have the correct permissions for the project

3. **Local testing issues**:
   - Ensure Firebase CLI is up to date: `npm install -g firebase-tools`
   - Check if port 5000 is already in use

## License

[Include license information here]

## Contact

For questions or support regarding this landing page, please contact [your contact information].
