ITI VAV MANAGEMENT SYSTEM - FREE ONLINE WEBSITE
================================================

WHAT I MADE
------------
This version keeps the same 14 ITI VAV modules from your existing system, but changes the storage from local SQLite to Supabase so the data can stay online. It also adds a login screen, reports, search, CSV export, SI edit, delete and mobile-friendly UI.

FILES
-----
1. index.html  -> complete website
2. schema.sql  -> database tables + security policies
3. README.txt  -> setup guide

FREE SETUP
----------
1. Create a free Supabase project at https://supabase.com/
2. Open SQL Editor in Supabase.
3. Paste the complete contents of schema.sql and Run it.
4. In Supabase Authentication -> Users, create your admin user (email + password).
5. In Supabase Project Settings -> API, copy:
   - Project URL
   - anon/public key
6. Open index.html in a text editor.
7. At the top of the <script>, replace:
   YOUR_SUPABASE_URL
   YOUR_SUPABASE_ANON_KEY
   with your Supabase values.
8. Upload the folder to GitHub.
9. Import the GitHub repository into Vercel or Netlify and deploy it.
10. Open the generated website link and login with the Supabase user.

IMPORTANT
---------
- Do NOT put a Supabase service_role/secret key in index.html. Only the anon/public key belongs in a browser app.
- The database is protected by Row Level Security and the included policy allows authenticated users only.
- If you want only ONE admin account, create only that user in Supabase and do not create other users.
- The current version does not migrate your old SQLite records automatically. Your old data can be imported separately into Supabase.

OLD SYSTEM -> ONLINE
--------------------
Old: Node.js + Express + SQLite
New: Static website + Supabase database + Supabase Auth
This means the website can run on free static hosting while the records remain online.

CUSTOMIZATION
--------------
To add your real ITI logo/banner, replace the CSS logo area or add image assets later. The app currently uses a clean built-in ITI VAV logo so it works immediately without extra image files.
