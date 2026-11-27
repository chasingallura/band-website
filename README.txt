CHASING ALLURA WEBSITE + PRIVATE CONTENT MANAGER
================================================

WHAT'S INCLUDED
- Responsive public band website (index.html)
- Exact Chasing Allura logo and supplied five-member band portrait in /assets
- Private CMS editor at /admin/ powered by Decap CMS
- Editable site settings, music releases, upcoming shows, merch, and photo/video gallery
- Content files in /content; uploads stored in /assets/uploads

IMPORTANT: THE ADMIN IS READY, BUT NOT YET CONNECTED OR LIVE
This package is prepared for Netlify + Git Gateway. It does not create a hosting account, GitHub repository, domain, or login by itself. The private login becomes active only after the deployment steps below. Do not share /admin as a public editing link until Invite-only access is enabled.

SETUP (ONE-TIME)
1. Create/sign in to a GitHub account and create a PRIVATE repository named chasing-allura-site.
2. Upload the contents of this folder to the repository's main branch (the folder contents, not the outer folder).
3. In Netlify, choose Add new site > Import an existing project > GitHub, select that repository, and deploy. Build command can be blank; publish directory is ".".
4. In the Netlify site dashboard, enable Identity. Set registration to Invite only. Invite only the people who should manage the band site.
5. Enable Git Gateway under Identity services.
6. Edit admin/config.yml and replace both YOUR-SITE-NAME.netlify.app values with the actual Netlify site URL. Commit that change to GitHub.
7. Open https://YOUR-SITE-NAME.netlify.app/admin/ and sign in using the invitation.
8. Add the band's real booking email and official social/streaming URLs in Site settings.

HOW TO EDIT AFTER SETUP
- Visit https://YOUR-SITE-NAME.netlify.app/admin/ and sign in.
- Use Music and releases to add singles/albums and streaming links.
- Use Upcoming shows to add dates, venues, times, and ticket links.
- Use Merchandise to add products, prices, photos, and store links.
- Use Photo and video gallery to add photos or YouTube links.
- Changes are committed to the connected repository and Netlify redeploys the public site.

DOMAIN
You can connect a purchased domain in Netlify > Domain management. chasingallura.com is the first name to check; its availability has not been verified.

BOOKING FORM
The current form opens the visitor's email app (mailto). A server-backed form that submits without an email app would require an additional form service or backend.

SECURITY
Use Invite only for CMS registration. Never put passwords, API keys, or private tokens in site files. The admin URL is not a substitute for authentication; Netlify Identity/Git Gateway must be enabled before real editing access is secure.
