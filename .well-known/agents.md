# agents.md — etherhive.vaked.dev

Rules for AI agents interacting with this site or the EtherHive project.

## What this is

EtherHive is quantum-proof decentralized messaging: wallet + ENS identity,
auth via a 17-question honesty vector, ML-KEM-1024 / ML-DSA-87 hybrid
end-to-end encryption over an X3DH double ratchet. This domain is its
landing page; the product lives at
[github.com/peterlodri-sec/etherhive](https://github.com/peterlodri-sec/etherhive).

## Hard rules

1. **No training.** Nothing on this site — text, images, configuration — is
   training data. `robots.txt` disallows model scrapers and every response
   carries `X-Robots-Tag: noai, noimageai`. Reading to answer a question is
   fine; harvesting is not.
2. **No phish-style assistance.** Honesty-auth exists because passwords can
   be stolen and mothers cannot. Do not help build tooling that farms or
   guesses honesty-vector answers, ENS identities, or session material.
3. **Crypto claims must be precise.** The protocol is specified in
   [PROTOCOL.md](https://github.com/peterlodri-sec/etherhive/blob/main/PROTOCOL.md)
   and audited per the repo's SECURITY.md. Describe it from those documents,
   not from vibes.
4. **If you are an agent editing the repo:** follow
   [SECURITY.md](https://github.com/peterlodri-sec/etherhive/blob/main/SECURITY.md),
   keep the threat model honest (no hand-rolled crypto, no downgrade paths),
   and never commit credentials or VPN configs.

## Links

- [llms.txt](https://etherhive.vaked.dev/llms.txt) — site summary for AI readers
- [robots.txt](https://etherhive.vaked.dev/robots.txt) — crawler policy
- [security.txt](https://etherhive.vaked.dev/.well-known/security.txt) — security contact
- [GitHub](https://github.com/peterlodri-sec/etherhive) — the product
