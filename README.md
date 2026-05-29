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

## Project structure

- `src/pages/BuildAdminTeam.tsx` — main screen and flow logic
- `src/components/` — header, admin row, invite button, toast
- `src/styles/tokens.css` — colours from the Figma design
- `docs/flow.md` — step-by-step behaviour notes

## Design source

Figma node `107:22922` (“cursor test” canvas) — four artboards left to right showing the invite flow.
