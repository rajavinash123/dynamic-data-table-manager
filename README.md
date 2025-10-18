This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
Frontend Interview Task 

 Dynamic Data Table Manager (Next.js + Redux + 
MUI) 

 Objective 
Build a Dynamic Data Table Manager using Next.js, Redux Toolkit, and Material UI 
(MUI). This project tests your ability to work with dynamic UIs, manage complex state, and 
implement real-world features like import/export, searching, sorting, and inline editing. 

 Project Requirements 

 Core Features 
1. Table View 
● Display a table with these default columns: 
Name, Email, Age, Role 
● Add sorting on column headers (ASC/DESC toggle) 
● Add global search (searches all fields) 
● Add client-side pagination (10 rows per page) 
2. Dynamic Columns 
● A "Manage Columns" modal: 
○ Add new fields like Department, Location 
○ Show/hide existing columns using checkboxes 
○ Reflect changes dynamically in the table 
● Persist column visibility in localStorage or Redux Persist 
3. Import & Export 
● Import CSV: 
○ Upload CSV, parse it using a library (e.g. PapaParse) 
○ Show errors for invalid format 
● Export CSV: 
○ Export current table view to a .csv file 
○ Only include visible columns 

 Bonus Features (Optional but appreciated) 
● 

 Inline row editing 
○ Double-click to edit fields inline 
○ Validate inputs (e.g., age must be a number) 
○ “Save All” and “Cancel All” buttons 
● 

 Row actions: Edit, Delete (with confirmation) 
● 

 Theme toggle (Light/Dark mode using MUI theming) 

 Column reordering via drag-and-drop 
 Fully responsive design 
 Tech Requirements 
● React 18 / Next.js 14 (App Router preferred) 
● Redux Toolkit for state management 
● Material UI (v5+) 
● TypeScript 
● React Hook Form for forms 
● PapaParse for CSV parsing 
●  FileSaver.js / Blob for export 
●  localStorage / Redux Persist for preferences 





solution 


🧩 Dynamic Data Table Manager

Tech Stack: Next.js 14 (App Router) | Redux Toolkit | Material UI (MUI v5) | TypeScript | React Hook Form | PapaParse | FileSaver.js

🚀 Objective

Build a Dynamic Data Table Manager that allows users to manage, filter, sort, import/export, and edit tabular data in a highly interactive and customizable way.

🧠 Features
🧾 1. Table View

Displays table with default columns: Name, Email, Age, Role

Sorting: Click column headers to toggle ASC/DESC

Global Search: Search across all fields

Pagination: 10 rows per page

⚙️ 2. Dynamic Columns

“Manage Columns” modal to:

Add new fields like Department or Location

Show/hide existing columns using checkboxes

Changes reflect dynamically in the table

Column visibility persisted using Redux Persist / localStorage

📁 3. Import & Export

Import CSV:

Upload CSV using PapaParse

Validation for invalid format

Export CSV:

Export current table view as .csv

Only visible columns included

💡 Bonus Features (Implemented / Optional)

✅ Inline row editing (double-click to edit, input validation)

✅ Edit / Delete row actions with confirmation modal

✅ Light / Dark theme toggle using MUI theming

✅ Column drag-and-drop reordering

✅ Fully responsive UI

🧱 Folder Structure
├── src/
│   ├── app/
│   │   ├── layout.tsx          # Root layout with providers
│   │   ├── page.tsx            # Home page
│   │   ├── providers.tsx       # Redux & Theme providers
│   │   └── globals.css         # Global styles
│   ├── components/
│   │   ├── DataTable.tsx       # Main table component
│   │   ├── EditRowDialog.tsx   # Edit row modal
│   │   ├── ColumnManagerDialog.tsx  # Manage columns modal
│   │   ├── ImportCSVDialog.tsx # CSV import modal
│   │   ├── DeleteConfirmDialog.tsx  # Delete confirmation modal
│   │   └── ThemeToggle.tsx     # Light/Dark mode toggle
│   ├── store/
│   │   ├── store.ts            # Redux store setup
│   │   ├── tableSlice.ts       # Table data slice
│   │   └── hooks.ts            # Typed Redux hooks
│   ├── types/
│   │   └── index.ts            # TypeScript interfaces
│   └── utils/
│       ├── csvUtils.ts         # CSV import/export helpers
│       └── tableUtils.ts       # Sorting & filtering utilities
├── package.json
├── tsconfig.json
├── next.config.js
└── README.md

🧰 Tech Stack
Technology	Purpose
Next.js 14	Frontend framework (App Router)
Redux Toolkit	State management
Material UI (MUI)	UI components
React Hook Form	Form validation
PapaParse	CSV import
FileSaver.js	CSV export
TypeScript	Type safety
localStorage / Redux Persist	State persistence
⚡️ Setup Instructions
1️⃣ Clone the Repository
git clonehttps://github.com/rajavinash123/dynamic-data-table-manager
cd dynamic-data-table-manager

2️⃣ Install Dependencies
npm install
# or
yarn install

3️⃣ Run the Development Server
npm run dev
# or
yarn dev


Open http://localhost:3000
 in your browser 🚀

🧑‍💻 Author

Avinash Kumar
Frontend Developer | Building scalable & interactive UIs

🏢 Submitted For

Surefy Technologies Pvt. Ltd. – Frontend Internship Assignment
