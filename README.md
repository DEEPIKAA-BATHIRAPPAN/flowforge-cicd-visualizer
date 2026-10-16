
# FlowForge — CI/CD Pipeline Visualizer

A responsive, interactive CI/CD pipeline simulation for learning and portfolio demos.

## Included
- Source → Build → Test → Staging → Production stages
- Live simulated logs and progress bar
- Toggle to simulate test failures
- Manual production approval or cancellation
- Run history, success rate, duration, and example workflow configuration
- No React, Vite, external libraries, or `npm install` required

## Run on Windows
1. Extract this ZIP.
2. Open the `flowforge-cicd-visualizer` folder in VS Code.
3. Open **Terminal → New Terminal**.
4. Run `npm run dev`.
5. Visit **http://localhost:5173**.
6. Press Ctrl+C to stop the local server.

Requires Node.js 18+ (Node.js 20+ recommended). The server uses Node's built-in modules only.

## Demo steps
1. Click **Run pipeline**.
2. Enable **Simulate test failure** and run again to show a failed Test stage.
3. Disable the failure toggle and run again.
4. Approve or cancel the production release when prompted.
5. Explore Run history and Configuration.

## Important
This is a **simulation**, not a real CI/CD system. It does not execute actual builds/tests or deploy to cloud infrastructure. The workflow YAML is illustrative. A future version can connect to GitHub Actions, GitLab CI, or Bitbucket Pipelines.

## Structure
- `index.html` — dashboard layout
- `styles.css` — styling and responsive layout
- `app.js` — interactive simulation
- `server.js` — dependency-free local web server
- `package.json` — run scripts
