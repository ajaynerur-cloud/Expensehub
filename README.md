# ExpenseHub V12

V12 preserves V11 rendering and features, and restores owner project controls.

## Owner controls
- Delete the entire project directly, without promoting another owner
- Promote a project member to owner
- Demote another owner while retaining at least one owner
- Disable or enable a project member
- Remove a member after owner password confirmation
- Complete-project delete removes the project, all project memberships, invitations, folders and transactions

## Preserved
Responsive mobile/tablet/desktop UI, Android safe-area, bottom navigation, transaction cards, login/signup, multi-project switcher, QR sharing, single add, mass add, desktop CSV/XLS/XLSX upload, Personal/Vendor/Received registers, folders, analytics, current/all Excel export, leave project, exit account, GitHub JSON storage and APK workflow.

Render build: `npm ci --no-audit --no-fund`; start: `npm start`.
