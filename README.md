# Next.js

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

[Configuration](https://codesandbox.io/docs/projects/learn/setting-up/tasks) has been added to optimize it for [CodeSandbox Projects](https://codesandbox.io/p/dashboard).

## Resources

- [CodeSandbox Projects — Docs](https://codesandbox.io/docs/projects)
- [CodeSandbox — Discord](https://discord.gg/Ggarp3pX5H)
- [Next.js — GitHub](https://github.com/vercel/next.js/)
- [Next.js — Docs](https://nextjs.org/docs)


## Firebase Analytics Integration

This project has been integrated with Firebase Analytics.

### Configuration

To enable Firebase Analytics, you need to add your Firebase project configuration:

1.  Open the file `lib/firebase.ts`.
2.  Replace the placeholder values in the `firebaseConfig` object with your actual Firebase project credentials:

    ```typescript
    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_AUTH_DOMAIN",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_STORAGE_BUCKET",
      messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
      appId: "YOUR_APP_ID",
      measurementId: "YOUR_MEASUREMENT_ID" // Optional: For Google Analytics 4
    };
    ```

### Features Implemented

*   **Automatic Page View Tracking:** Page views are automatically tracked and sent to Firebase Analytics whenever a user navigates to a new page. This is handled in `pages/_app.tsx`.
*   **Custom Event Logging Example:** An example of how to log custom events is provided in `pages/index.tsx`. You can find a button labeled "Log Custom Event" that demonstrates this functionality.
