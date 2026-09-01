# Study Buddy MCQ v2

This version uses a real online database (Supabase), so quizzes published by the admin are available to other devices.

## Setup

1. Create a free Supabase project.
2. Open SQL Editor and run `supabase.sql`.
3. In Supabase Project Settings > API, copy:
   - Project URL
   - anon/public key
4. Open `index.html` and replace:
   - `PASTE_YOUR_SUPABASE_URL`
   - `PASTE_YOUR_SUPABASE_ANON_KEY`
   - `CHANGE_THIS_PASSWORD`
5. Put `index.html` on GitHub Pages.

## Important security note

This is a prototype. The admin password is stored in browser JavaScript, and the database policies allow public insert/delete. Do NOT use this design for sensitive/private information.

For a proper Version 3, use Supabase Authentication + Row Level Security so only you can create/delete quizzes while students can only read quizzes and submit attempts.

## Free

Supabase has a free tier, and GitHub Pages can host static sites for free, subject to their current limits/terms.
