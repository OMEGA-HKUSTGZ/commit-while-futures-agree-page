# Commit While Futures Agree — OMEGA Lab project page

Project page for **Commit While Futures Agree: Consequence-Aware Adaptive Action Chunking for Robot
Manipulation** (CA³C), in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2610.07949>
- Page: <https://omega-hkustgz.github.io/projects/commit-while-futures-agree/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/`; there is no build step. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs
node tools/serve.mjs     # look at it locally
```

Every pull request gets a preview link, posted on the pull request. A push to `main` asks the
lab site to republish.

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2610.07949v1 (6 Oct 2026). The text paraphrases the abstract and Sections 1, 3, 4 and 5, with K = 3 from the appendix; it adds no claims. |
| `teaser.webp`, `framework.webp`, `adaptive-commitment.webp`, `failure-to-success.webp`, `horizon-distribution.webp`, `real-world.webp` | Figs. 1–6 of the paper, rendered from the arXiv source PDFs at 2400 px wide (`pdftoppm`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| LIBERO, LIBERO-Plus, RoboCasa and real-robot tables, headline numbers | Tables 1, 2, 3 and 6 of the paper, copied from the LaTeX source. Bracketed changes are the paper's own. Ablation numbers in the text are from Section 4.3 (Tables 4 and 5). |
| Evidence labels | Fig. 4 is a simulated LIBERO rollout pair (Simulation); Fig. 6 shows the AgiBot G2 tasks of Section 4.5 (Real-world). |

Not on the page because no public material exists: a code repository (so there is no Code
button), demo video, and released world-model weights. The ablation tables (Tables 4 and 5) are
left to the paper.
