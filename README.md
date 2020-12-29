# Startup Web App

Serverless web application to test startup ideas.

## Prerequisites

- Install node version manager and the latest npm version

```bash
    curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
    source ~/.zshrc
    nvm install node
    nvm use node
```

- Install firebase tools and the vue cli globally on your machine

```bash
    npm install firebase-tools -g
    npm install vue-cli -g
```

## Test locally

```bash
    firebase serve
```

## Deploy

- Build the web application

```bash
    cd public && npm run build && cd ..
```

- Deploy everything to GCP

```bash
    firebase deploy --only hosting
```