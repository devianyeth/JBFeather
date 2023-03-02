# Juicebox x Feather test

# Setup

## Install

```bash
yarn
```

## Keyp Setup

1. Copy the file `.sample-env` to `.env`
2. Create a new application on on https://dev.usekeyp.com.

- Set the redirect URI to `http://localhost:3000/api/auth/callback/keyp` (note that your port may be different). Ready for production? Make sure to upate this to eg. `https://my-site.com/api/auth/callback/keyp`.
- Copy the "CLIENT ID" for your application and set it to `KEYP_CLIENT_ID` in `.env`

3. In the `.env`, set `TOKEN_SECRET` to a random string, which is used for `next-auth` session cookies. You can generate this using `openssl rand -base64 32`. (NOTE: Do not use your access token here)

# Run

```bash
yarn dev
```
