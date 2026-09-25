# ExpenseHub V11

V11 preserves the complete V10.1 feature set and adds adaptive layouts for installed Android, mobile web, tablets, laptops and large desktops.

## Responsive design
- Safe-area viewport support for Android edge-to-edge and display cutouts
- Mobile top bar, off-canvas navigation, tap scrim and fixed bottom navigation
- Transaction cards on phones instead of compressed desktop tables
- Horizontally scrollable mass-entry and file-preview tables
- Two-column tablet grids and three-column desktop grids
- Touch targets of at least 44px, mobile number keyboard hints and responsive dialogs
- Sticky desktop/tablet project header and navigation

## Preserved features
Login/signup, multi-project personal/shared accounts, QR join-or-create-own flow, project switching, single add, mass add, desktop CSV/XLS/XLSX upload, preview/edit/selection/folder/type assignment, isolated Personal/Vendor/Received registers, folders, folder analytics, current/all-project Excel export, project leave with contribution deletion, full-account exit, GitHub JSON storage, Capacitor Android and GitHub Actions APK build.

## Render
Build: `npm ci --no-audit --no-fund`; Start: `npm start`.
Variables: NODE_VERSION=22, GITHUB_OWNER, GITHUB_REPO, GITHUB_BRANCH=main, GITHUB_DATA_PATH=data/expense-data.json, GITHUB_TOKEN, JWT_SECRET, APP_BASE_URL.
