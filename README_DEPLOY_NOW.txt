ITI VAV - DEPLOY NOW

1. Create a Supabase project.
2. In Supabase SQL Editor, paste and run schema.sql.
3. Create a user in Authentication > Users.
4. Open index.html and replace:
   YOUR_SUPABASE_URL
   YOUR_SUPABASE_ANON_KEY
   with your Supabase Project URL and anon/public key.
5. Upload the whole folder to a GitHub repository.
6. In Vercel, Import the GitHub repository and Deploy.
7. Your live URL will be similar to:
   https://iti-vav.vercel.app

IMPORTANT:
- Do NOT put the Supabase service_role/secret key in index.html.
- Use only the public anon/publishable key.
- The existing SQLite database is not automatically migrated by this package.
