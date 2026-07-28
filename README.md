# traverse-assets

**Public marketing assets for RTS Traverse, LLC.** Social post graphics, and nothing else.

This repository is **public on purpose**. It exists for one reason: Buffer fetches post media from
a public HTTPS URL at publish time and accepts no binary upload, so every graphic that goes out on
LinkedIn, Instagram, or Facebook has to live at an address anyone can reach.

## What belongs here

- Rendered social post graphics (PNG), under `social/{YYYY}/{MM}/{slug}.png`

## What does not belong here — ever

- Client names, client work, logos, screenshots, or deliverables
- Anything PHI-adjacent. Our healthcare clients operate under HIPAA; this repo is public and
  is never an appropriate home for anything touching them.
- Source code, internal documents, strategy, pricing, contracts
- Credentials of any kind

Everything internal lives in `rts-traverse/traverse-os` (private). Everything about the website
lives in `rts-traverse/traverse-site` (private). **If you are unsure whether something belongs in
this repo, it does not.**

## How a graphic gets here

Graphics are produced in `traverse-os` — a generated backdrop composited under a deterministic
HTML/CSS brand layer — and only the finished PNG is copied here. See
`company/marketing/social-setup/pipeline-smoke-test.md` in that repo for the full pipeline.

The imagery in these graphics is AI-generated. We disclose that on the posts themselves.

## Serving

GitHub Pages serves `main` from the repo root, so a file at `social/2026/07/example.png` is
reachable at:

```
https://rts-traverse.github.io/traverse-assets/social/2026/07/example.png
```

This is an **interim** host. The intended long-term home is `traverserts.com/social/…`; moving
there is a path change in one field of a post's frontmatter, not a pipeline change.

---

© RTS Traverse, LLC
