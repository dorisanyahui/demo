
---

```markdown
# CPSY 350 Github Action CI Project

This project is a Node.js application created as part of the CPSY 350 course assignment. It demonstrates Continuous Integration (CI) and Continuous Deployment (CD) using GitHub Actions and Docker.

---

## 📦 Project Structure

```

demo/
├── server.js              # Main Node.js server
├── package.json           # Project configuration and dependencies
├── test/                  # Mocha test cases
│   └── test.js
├── Dockerfile             # For Docker build
├── .github/
│   └── workflows/
│       └── github-actions-demo.yml  # GitHub Actions CI/CD config
└── README.md

````

---

## 🚀 How to Run the App Locally

1. Install dependencies:
   ```bash
   npm install
````

2. Start the server:

   ```bash
   npm start
   ```

3. Open your browser at:

   ```
   http://localhost:3000
   ```

---

## 🧪 How to Run Tests

The project uses **Mocha** for testing.

```bash
npm test
```

---

## 🐳 Docker Instructions

### Build Docker Image

```bash
docker build -t cpsy350-app .
```

### Run the Docker Container

```bash
docker run -p 3000:3000 cpsy350-app
```

Then visit:

```
http://localhost:3000
```

---

## 🔁 GitHub Actions Workflow

This project includes a CI/CD pipeline via GitHub Actions:

* `build-and-test`:

  * Installs dependencies
  * Runs test cases using Mocha

* `build-and-push`:

  * Builds a Docker image
  * Pushes it to Docker Hub using secrets

### Secrets Used in GitHub Actions

* `DOCKER_USERNAME`
* `DOCKER_TOKEN`

> 🔐 Set these under your repo’s Settings > Secrets and variables > Actions.

---

## ✅ Output Example

When running the app, you will see:

```
CPSY-350 Project: Github Actions CI. SAIT-ID:000123456
```

> Replace `000123456` with your actual SAIT ID if needed.

---


