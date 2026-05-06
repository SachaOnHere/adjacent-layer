# The Adjacent Layer — Jim

A demo built for Hank Massey / Day Pitney.

## Deploy to Vercel

1. Push this folder to a GitHub repo
2. Import the repo in Vercel
3. In Vercel project settings → Environment Variables, add:
   - Name: `ANTHROPIC_API_KEY`
   - Value: your Anthropic API key
4. Deploy

The app reads the API key from the Vercel environment at runtime.
It does NOT store any conversation data — all sessions are ephemeral.

## What it does

A single-page chat interface powered by Claude, configured as "Jim" —
a senior M&A advisor with 25 years in sell-side mandates for closely-held
industrial manufacturing businesses. Pre-loaded with the surgical mesh /
knee replacement client context.

Jim leads with his three current observations before Hank asks anything.
He doesn't hedge. He doesn't validate premises. He leads with the
counterargument. He ends every response with a specific next action.

## To adapt for a different mandate

Edit the SYSTEM_PROMPT constant in index.html:
- Change the mandate context (THE CURRENT MANDATE section)
- Update Jim's current read (YOUR CURRENT READ ON THE DEAL section)
- Update the opening items in the HTML (the three numbered observations)
- Update the mandate-bar text in the header

The rest of the prompt stays the same across mandates.
