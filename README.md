# Multi Store Price Portal (Vercel + Supabase)

## Deploy
1. Create a Supabase project and copy the **Transaction pooler** database URL.
2. Upload this project to GitHub and import it in Vercel.
3. Add all variables from `.env.example` in Vercel Project Settings > Environment Variables.
4. Deploy. Tables are created automatically on first request.
5. Open `/developer/login`, create stores and their users.
6. Download each store's Local Bridge ZIP from Developer Portal.

## Important
- Store records are separated by `store_id`.
- Data lives in Supabase PostgreSQL, not Vercel local storage, so redeploy/sleep does not delete it.
- Change the default developer password before production.
- For high security, restrict the Supabase database password and rotate it if exposed.
