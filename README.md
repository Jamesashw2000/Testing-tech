# Admin invite flow prototype

Interactive prototype of the **Add / Invite Admins** step from the easyfundraising cause registration journey, based on the Figma file [Add-invite-Admins-to-cause-reg-journey](https://www.figma.com/design/g5IfKUrbfDuagu8n0jhqEE/Add-invite-Admins-to-cause-reg-journey?node-id=107-22922).

## What this does

Walks through the four screens in your Figma flow:

1. **Empty** — placeholder in the email field
2. **Typing** — user enters an email; Invite becomes active
3. **Loading** — spinner on the Invite button while sending
4. **Success** — invited person appears with “Invite sent”, field clears, green toast appears

## Run locally

```bash
cd admin-invite-flow
npm install
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

## Deploy on Vercel

1. Push this folder to GitHub. The repo must include the **`src`** folder (check on github.com that you see `src/pages`, `src/components`, etc.).
2. In Vercel → **Import Project** → select the repo.
3. **Root Directory:**
   - If the repo contains only this app (you see `package.json` at the top level): leave Root Directory **empty** / `.`
   - If the repo is a parent folder and this app lives inside `admin-invite-flow`: set Root Directory to **`admin-invite-flow`**
4. Build Command: `npm run build` · Output Directory: `dist`
5. Deploy.

If build fails with “No inputs were found”, the `src` folder is missing from GitHub or the Root Directory is wrong.

## Project structure

- `src/pages/BuildAdminTeam.tsx` — main screen and flow logic
- `src/components/` — header, admin row, invite button, toast
- `src/styles/tokens.css` — colours from the Figma design
- `docs/flow.md` — step-by-step behaviour notes

## Design source

Figma node `107:22922` (“cursor test” canvas) — four artboards left to right showing the invite flow.
