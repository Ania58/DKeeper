# dKeeper

Welcome to dKeeper, a decentralized note-keeping application built with Motoko (for the backend) and React (for the frontend) on the Internet Computer.

## 📌 Project Overview

dKeeper allows users to create, read, and delete notes that are stored on a decentralized backend. The frontend is built using React, and the backend logic is implemented in Motoko.

## 🏗️ Tech Stack

Motoko – Smart contract language for the Internet Computer.

React – Frontend framework for a dynamic UI.

Webpack – Bundler for the frontend.

DFINITY SDK – Tools for deploying and interacting with Internet Computer canisters.

Material-UI – Used for UI components.

## 🚀 Getting Started

1️⃣ Install DFINITY SDK

Make sure you have the DFINITY SDK installed on your system:

```bash
sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"
```

2️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/dkeeper.git
cd dkeeper
```

3️⃣ Start the Internet Computer Local Replica

```bash
dfx start --background
```

4️⃣ Deploy Canisters

```bash
dfx deploy
```

5️⃣ Run the Frontend

```bash
npm install
npm start
```

This will start the development server at http://localhost:8080/, while the backend API runs on http://localhost:8000/.

## 🔧 Project Structure

```
dkeeper/
├── dist/                      # Build output directory
├── node_modules/              # Installed dependencies
├── src/                       # Main source code
│   ├── declarations/          # Auto-generated canister bindings
│   │   ├── dkeeper/           
│   │   │   ├── dkeeper.did.d.ts
│   │   │   ├── dkeeper.did.js
│   │   │   ├── dkeeper.most
│   │   │   ├── dkeeper.old.did
│   │   │   ├── dkeeper.old.most
│   │   │   ├── index.js
│   ├── dkeeper/               # Motoko backend logic
│   │   ├── main.mo            # Smart contract logic
│   ├── dkeeper_assets/        # Frontend React app
│   │   ├── assets/            # Static (icons, styles)
│   │   │   ├── favicon.ico
│   │   │   ├── logo.png
│   │   │   ├── sample-asset.txt
│   │   │   ├── styles.css
│   │   ├── src/               # React source code
│   │   │   ├── components/    # React components
│   │   │   │   ├── App.jsx
│   │   │   │   ├── CreateArea.jsx
│   │   │   │   ├── Footer.jsx
│   │   │   │   ├── Header.jsx
│   │   │   │   ├── Note.jsx
│   │   │   ├── index.html   # Entry HTML file
│   │   │   ├── index.jsx    # React entry point
├── .gitignore               # Git ignore file
├── dfx.json                 # Internet Computer config
├── package.json             # Dependencies and scripts
├── package-lock.json        # Dependency lock file
├── webpack.config.js        # Webpack setup
└── README.md                # Project documentation
```

## 🛠️ Features

* ✅ Create notes
* ✅ View all saved notes
* ✅ Delete notes
* ✅ Persist data using Internet Computer smart contracts

## 📌 Deployment to the Internet Computer

If you want to deploy your project live on the Internet Computer, use:

```bash
dfx deploy --network ic
```

This will deploy the canisters to the IC mainnet.

## 📝 Additional Resources

Internet Computer Docs https://internetcomputer.org/docs/home

Motoko Language Guide https://internetcomputer.org/docs/motoko/main/getting-started/motoko-introduction

React Documentation https://react.dev/

## 💡 Future Improvements

✅ Add user authentication

✅ Implement note editing

✅ Improve UI styling