# Public API and Config Notes

This branch only documents configuration names. It must not contain real keys.

## Public Client Variables

```text
VITE_FIREBASE_API_KEY=dummy-firebase-api-key
VITE_FIREBASE_AUTH_DOMAIN=dummy-project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=dummy-project-id
VITE_FIREBASE_STORAGE_BUCKET=dummy-project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=000000000000
VITE_FIREBASE_APP_ID=1:000000000000:web:0000000000000000000000
VITE_SUPABASE_URL=https://dummy-project.insforge.app
VITE_SUPABASE_ANON_KEY=dummy-anon-key
VITE_PUBLIC_SUPPORT_EMAIL=support@example.com
```

## Server Secrets

Server secrets should be configured in provider dashboards, CI secrets, or Firebase Functions secrets.

Examples:

```text
OPENROUTER_API_KEY=dummy-openrouter-key
GEMMA_API_KEY=dummy-server-ai-key
ADMIN_BUGS_SECRET=dummy-admin-secret
```

## Safety Rule

If a value grants write access, admin access, billing access, model quota access, or long-lived user access, never commit it.
