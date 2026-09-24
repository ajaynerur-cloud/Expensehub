# ExpenseHub V5

Platform-specific rebuild designed to avoid the previous Connecting screen. The dashboard renders before any network request, no APP_KEY is used, no service worker is registered, and versioned CSS/JS filenames prevent stale-cache problems.

## Render Web Service
Create New > Web Service. Build command: `npm install`. Start command: `npm start`. Environment variables: `NODE_VERSION=22`, `GITHUB_OWNER`, `GITHUB_REPO`, `GITHUB_BRANCH=main`, `GITHUB_DATA_PATH=data/expense-data.json`, `GITHUB_TOKEN`. Do not add APP_KEY.

## Replace old deployment
Delete all old repository files first, then upload all V4 files to the repository root. In Render use Manual Deploy > Clear build cache & deploy. After deploy open the site with `?v=4` and hard refresh.

## CSV import
Import CSV opens the Android/browser file chooser. Review and edit rows, select rows, assign a register and folder in bulk or individually, then save. The included `docs/payments-sample.csv` matches the uploaded payments format.

## APK
The included Capacitor config points to `https://expensehub-api.onrender.com`. Run the GitHub Action `Build Android APK` and download the artifact.


## Platform-specific entry options

Desktop web:
- Load Excel/CSV file
- Single expense add
- Mass expense add

Installed Android app:
- Single expense add
- Mass expense add
- The file-upload menu is hidden in the native app

Mass add starts with five editable rows and supports adding more rows, bulk register assignment, bulk folder assignment, validation, selection, and one-save submission.
