# Ahad Ali Wedding Invitation

Static site (plain HTML, CSS and JavaScript). No build step, no dependencies.

## Files
- `index.html` : the invitation (envelope, events, countdown, directions)
- `share.html` : private link maker, open it at `/share`
- `vercel.json` : enables clean URLs so `/share` works

## Deploy
Push to GitHub, import the repo in Vercel, framework preset "Other", leave build command and output directory empty.

## Personal links
Open `/share`, type the guest or family name, choose the events, then copy the link or send it on WhatsApp.

Link format:
- `/?for=Ramzan%20and%20family&events=walima`
- `events` accepts `mehandi`, `barat`, `walima` (comma separated). Leave it out to show all three.
- `for` is the name shown on the envelope and the invitation.

## Edit details
Dates, times and addresses are in `index.html`. The countdown times are in the `events` array in the script near the bottom (Pakistan time, +05:00). Walima and Mehandi map links are in the event cards and in the Venue section.

## Owner shortcut
Open `/share` once in your own browser. After that, a small "Share this invitation" button appears on the invitation, only in that browser, and takes you back to the link maker. Guests never see it.
