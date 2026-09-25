# ExpenseHub V9

V9 uses one user login with multiple independent expense projects.

## Project model
- Every registered user can create personal projects at any time.
- A user can own multiple projects and join multiple shared projects.
- Project folders, transactions, members, analytics, invitations and deletion are isolated by `projectId`.
- The top project selector switches between projects without another login.
- The All Projects page lists personal and shared projects in separate cards with per-project roles.

## Invitation flow
When a signed-in user opens a valid invitation, ExpenseHub presents two explicit choices:
1. Join the invited existing project.
2. Create a separate personal project.

Creating a personal project does not remove the invitation. The user can return and join the invited project. After joining, both projects appear in the project selector and project home.

## Render Web Service
Build: `npm ci --no-audit --no-fund`
Start: `npm start`

Required variables: `NODE_VERSION=22`, `GITHUB_OWNER`, `GITHUB_REPO`, `GITHUB_BRANCH=main`, `GITHUB_DATA_PATH=data/expense-data.json`, `GITHUB_TOKEN`, `JWT_SECRET`, `APP_BASE_URL`.

## Android
The package includes matching `package.json`, `package-lock.json`, Capacitor 8.5.0, and a GitHub Actions APK workflow.
