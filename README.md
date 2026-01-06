# GD Collabs
(THE REST OF THE REPO WILL BE ADDED SOON BE PATIENT)
this is my geometry dash megacollab site. basically lets people create collabs, join parts, chat in forums, all that stuff.

## what it does

- create collabs with parts, deadlines, songs, all that
- join parts and work on them
- forums for each collab (with markdown, emojis, images, videos)
- applications to join collabs
- kick/ban system with appeals
- bug reports
- api for getting collab data
- discord oauth login
- gd username linking with gdbrowser

## tech stuff

- cloudflare workers (serverless backend)
- cloudflare d1 (sqlite database)
- react for frontend
- discord oauth for login

## setup

1. clone this repo
2. `npm install`
3. set up your cloudflare worker and d1 database
4. run migrations: `wrangler d1 migrations apply DB`
5. set secrets in cloudflare dashboard:
   - `DISCORD_CLIENT_ID`
   - `DISCORD_CLIENT_SECRET`
   - `TURNSTILE_SECRET_KEY` (optional)
6. `npm run deploy`

thats pretty much it. the code is pretty straightforward, just look around if you need to change stuff.

## features

- organic/natural ui design (blobs, grain textures, all that)
- responsive design (works on mobile)
- markdown support in forums
- image/video uploads
- emoji support
- api with basic auth
- rate limiting
- security headers
- input sanitization

thats about it. if you have questions just look at the code, its pretty self explanatory.

