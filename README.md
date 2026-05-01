# Denver Odor Pros Website

Static multi-page website for Denver Odor Pros, a Denver ozone odor removal business.

Open `index.html` in a browser to preview locally. All call buttons use `tel:303-882-2989`.

## Lead Email Backend

Estimate forms and chat estimate requests submit to `/api/estimate`, a Vercel serverless function that emails leads to `denverodorpros@gmail.com` through Resend.

Set these Vercel environment variables before relying on live form submissions:

- `RESEND_API_KEY`: your Resend API key.
- `LEAD_TO_EMAIL`: `denverodorpros@gmail.com`
- `LEAD_FROM_EMAIL`: use `Denver Odor Pros <onboarding@resend.dev>` for testing, then switch to a verified sender such as `Denver Odor Pros <denverodorpros@gmail.com>` after the domain is verified in Resend.
