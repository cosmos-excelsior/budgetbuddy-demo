# BudgetBuddy — Vercel presentation demo

By BuddyTech Solutions. Prepared for the Technical Communication product launch presentation.

## What works
- Manual income/expense entry, edit and delete
- Monthly balance and category breakdown
- Savings targets and progress
- Individual installment reminders and paid status
- Temporary sample-data mode for presentations
- Browser-local saving outside sample-data mode

There is no sign-in, database, bank connection, payment processing or cross-device syncing. Each visitor has their own records in their browser. Clearing browser data removes those records. Sample-data changes are temporary. Installments are in-app reminders only; marking paid does not create an expense. Goal progress is independent of the balance.

## Deploy using GitHub and Vercel
1. Extract this ZIP.
2. Create a GitHub repository named `budgetbuddy-demo`.
3. Upload the contents of the extracted folder to the repository root. `package.json`, `index.html`, and `vercel.json` must be at the root, not inside an extra folder. Include `app`, `components`, `lib`, `public`, and `vendor`.
4. Sign in at https://vercel.com/new and import that repository.
5. Framework: Vite. Build command: `npm run build`. Output directory: `dist`. Install command: `npm install`. Use Node.js 22.x or a newer supported version. No environment variables are needed.
6. Click Deploy. Vercel supplies the final URL when it succeeds. Test the production link in a private window before sending it to your professor.

## Deploy from your computer instead
Install Node.js 22.13+ first. Open a terminal inside this folder:

```sh
npm install
npm run build
npx vercel login
npx vercel --prod
```

Choose your account, create a new project, and accept the Vite settings. Follow Vercel's login flow in your browser. Do not paste passwords or access tokens into chat.

## Presentation walkthrough
1. Click Try sample data.
2. Explain the dashboard balance, income and spending categories.
3. Add an expense and show the totals change.
4. Open Savings goals, edit a goal and update the saved amount.
5. Open Installments and mark a payment paid.
6. Exit demo to return to browser-saved entries. Enter demo again to restore the original samples.

## Local preview
```sh
npm install
npm run dev
```
Open the address printed in your terminal. The supplied `dist` folder is the tested production build, but Vercel will rebuild from source.

## Validation
The production Vite build passed. Browser interaction testing and Vercel account deployment have not been completed in this environment.

## AI disclosure
AI assistance was used to generate and adapt the website code and presentation demo. The group should review the content and demonstrate the features before submission.

## References
https://vercel.com/docs/frameworks/frontend/vite
https://vercel.com/docs/cli/deploy
