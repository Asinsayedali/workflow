# cc-f1e3b118-2899-453c-aef7-b46035bd28be — exported from N2C

This is a standalone Wrangler project. N2C is not involved from here on — the
compiled script in `src/index.ts` is exactly what N2C would deploy for this workflow.

## Deploy

1. `npm install` (installs the Wrangler toolchain from `package.json`).
2. `npx wrangler login` (if you haven't already).
3. Set each required secret: `npx wrangler secret put CREDENTIAL_GOOGLE_CALENDAR_1`, `npx wrangler secret put CREDENTIAL_GMAIL_1`.
   For local dev, copy `.dev.vars.example` to `.dev.vars` and fill in real values.
4. `npx wrangler deploy`.

## Required secrets

- `CREDENTIAL_GOOGLE_CALENDAR_1`
- `CREDENTIAL_GMAIL_1`
