# Deploy node.js app in Google App Engine using Github Action

> This project demonstrate how to deploy node.js sample app in Google App Engine using Github Action

## 🚀 Features

- ✨ Google cloud acount setup
- ⚡ App Engine
- 🔒 How to deploy node app from local

## 🛠 Tech Stack

- Node.js
- Express
- Google Cloud(App Engine)

## 🧑‍💻 Local Setup
- Enable App Engine, App Engine Admin API, Cloud Build
- Create a service account(with permission App Engine Admin, Cloud Build Editor, Storage Admin, Service Account User), create a key, download the key in local
- In Google Cloud console select App Engine and create application in any region(this is one time activity and has to do manually)
- Add GitHub Secrets to your repo:  Repo → Settings → Secrets and variables → Actions → New repository secret as GCP_SA_KEY = contents of key.json (JSON string)
- Create a simple node.js app with app.yaml
- Create a .github/workflows/deploy.yml file in root of your node app
- When you push to GitHub, app will be deployed to App Engine

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/rupachowrasia/node-gcp-app-engine-deploy-with-github-action.git

# Move into the project directory
cd node-gcp-app-engine-deploy-with-github-action

# Install dependencies
npm install

# Run the app
npm run start
