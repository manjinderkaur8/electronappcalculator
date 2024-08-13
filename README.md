# Wi-Jungle Electron App

## Project Overview
The Wi-Jungle Electron App is a desktop application developed using Electron, inspired by a provided Figma design. The application features a login page and a scientific calculator page. The backend processing is handled using C++ to ensure fast and efficient operations, while the front-end interface is crafted using HTML, CSS, and JavaScript.

## Features
- Login Page: A user-friendly login form with basic validation.
- Scientific Calculator: A fully functional calculator with various scientific functions.
- Electron Integration: The application is packaged as a native desktop application using Electron.
- C++ Backend: The backend logic is implemented in C++ for enhanced performance.

## Project Structure
```
Wi-Jungle-Electron-App/
│
├── main.js               # Main Electron process script
├── index.html            # Login page HTML
├── calculator.html       # Calculator page HTML
├── renderer.js           # JavaScript for handling UI interactions
├── styles.css            # CSS for styling the application
├── package.json          # Project metadata and dependencies
├── C++                   # Directory for C++ backend files
│   ├── backend.cpp       # C++ backend logic
│   └── ...               # Additional C++ files if any
├── assets/
│   ├── illustration.png  # Image used on the login page
│   ├── user.jpg          # Placeholder for user profile picture
│   └── ...               # Other images/assets
└── README.md             # Project documentation (this file)
```

## Installation

### Prerequisites
- Node.js (latest stable version recommended)
- npm (comes with Node.js)
- C++ compiler (e.g., GCC for Linux/MacOS, MSVC for Windows)

### Setup Instructions

1. Clone the Repository:
   ```bash
   git clone https://github.com/manjinderkaur8/electronapp.git
   cd electronapp
   ```

2. Install Node.js Dependencies:
   ```bash
   npm install
   ```

3. Build the C++ Backend:
   Navigate to the `C++` directory and compile the backend code:
   - Linux/MacOS:
     ```bash
     g++ -o backend backend.cpp
     ```
   - Windows:
     ```bash
     cl /EHsc backend.cpp
     ```

4. Start the Electron Application:
   ```bash
   npm start
   ```

## Building the Application

To package the Electron app into an executable, use the `electron-packager`:

```bash
npx electron-packager . WiJungleApp --platform=win32 --arch=x64 --out=dist/
```

This command packages the application for Windows 64-bit architecture. Adjust the `--platform` and `--arch` flags accordingly if you're targeting other operating systems or architectures.

## Usage

### Login Page
- Login: Enter the cloud, username, and password to access the calculator.
- Validation: Ensure all fields are filled before logging in.
![image](https://github.com/user-attachments/assets/ae4fda46-00b9-40ad-9972-0c09724305fa)

### Calculator
- Basic and Scientific Functions: Perform calculations such as addition, subtraction, trigonometric functions, logarithms, and more.
- Clear Screen: Use the `AC` button to clear the input.
- ![image](https://github.com/user-attachments/assets/9f3d398d-b3a9-4376-a8f5-ac1a7f21f3f5)


## Development Guide

### Adding New Features
- Frontend (UI): Modify the `index.html`, `calculator.html`, and `styles.css` files to change the UI.
- JavaScript Logic: Update `renderer.js` to add new interactions or modify existing ones.
- Backend (C++ Logic): Add or update the C++ files in the `C++` directory to modify backend functionality.

### Debugging
- Developer Tools: Open Electron's Developer Tools with `Ctrl+Shift+I` (Windows/Linux) or `Cmd+Option+I` (Mac) for debugging.

## Contributing

If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are welcome and appreciated!

## License

This project is made by Manjinder Kaur, you can contact me through this https://manjindersportfolio-2a444e.webflow.io/

