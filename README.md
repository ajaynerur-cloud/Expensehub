# ExpenseHub V13

V13 fixes invite registration and preserves the V12 responsive and owner-control functionality.

## Invite authentication flow
- An unauthenticated invitee sees the invited project and can create an account or sign in.
- Account creation returns a JWT and signs the invitee in immediately.
- The invite remains in the URL/session and the signed-in invitee is shown the choice to join the invited project or create a separate personal project.
- Joining consumes the one-time invitation and immediately opens the joined project.

## Branding
The user-supplied ExpenseHub image is included as `public/assets/app-icon.png`, `assets/icon.png`, `assets/icon-only.png`, and `assets/icon-foreground.png`. The page favicon and header use it. The Android workflow runs `@capacitor/assets` before the APK build to generate Android launcher resources.

## Preserved capabilities
Responsive Android/mobile/tablet/desktop rendering, signup/login, multi-project personal/shared accounts, QR invites, project switching, single add, mass add, desktop CSV/XLS/XLSX import, separate Personal/Vendor/Received registers, folders, analytics, member promotion/disable, complete-project deletion, current/all Excel export, GitHub JSON storage and APK workflow.

Render build: `npm ci --no-audit --no-fund`; start: `npm start`.
