# etherhive.vaked.dev

Landing page for [EtherHive](https://github.com/peterlodri-sec/etherhive) — quantum-proof decentralized messaging, wallet + ENS identity, auth via honesty.

Live URL: **[https://etherhive.vaked.dev](https://etherhive.vaked.dev)**

Static single-file site, no build step, no JavaScript. Deployed to Cloudflare Pages
(project `etherhive-vaked-dev`) — push to `main` triggers `.github/workflows/deploy.yml`.

## One-time CI secret

The workflow deploys with `wrangler pages deploy` and needs a scoped API token
as a repo secret (the Pages project itself was created by direct upload, so CI
has never been able to deploy without it):

1. Cloudflare dashboard → **My Profile → API Tokens → Create Token**
   → "Create Custom Token"
2. Permissions: **Account → Cloudflare Pages → Edit** (account `5b8d…5940`),
   no zone permissions needed
3. `gh secret set CLOUDFLARE_API_TOKEN` (or repo Settings → Secrets)

`CLOUDFLARE_ACCOUNT_ID` is already set. Without the token, deploys run
locally via `npx wrangler pages deploy _site --project-name=etherhive-vaked-dev`
(any authenticated wrangler).

## Ship list (nothing else leaves the repo)

`index.html`, `404.html`, `favicon.svg`, `robots.txt`, `site.webmanifest`,
`llms.txt`, `_headers`, `icon-192/512.png`, `apple-touch-icon.png`,
`og-image.png/svg`, `.well-known/agents.md`, `.well-known/security.txt`.

## Sister sites

- ✦ [vaked.dev](https://vaked.dev)
- ✦ [bonfire.vaked.dev](https://bonfire.vaked.dev)
- ✦ [qwave.vaked.dev](https://qwave.vaked.dev)
- ✦ [music.vaked.dev](https://music.vaked.dev)
- ✦ [art.vaked.dev](https://art.vaked.dev)
- ✦ [pocoo.vaked.dev](https://pocoo.vaked.dev)
- ✦ [lovetta.vaked.dev](https://lovetta.vaked.dev)
- ✦ [store.vaked.dev](https://store.vaked.dev)
- ✦ [proposal.vaked.dev](https://proposal.vaked.dev)
- ✦ [quant-love](https://mlxquantlovefrom.com)
- ✦ [portail.vaked.dev](https://portail.vaked.dev)
- ✦ [axiomquant.org](https://axiomquant.org)
- ✦ [peterl.dev](https://peterl.dev)
