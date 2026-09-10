# Chinese CAPTCHA Practice

A single-page, dependency-free practice tool covering thirteen CAPTCHA styles deployed on Chinese sites — click-sequence, idiom completion, word order, icon click, rotate-to-align, arithmetic, match-3, gomoku, grid selection, and mouse-trajectory obstacle avoidance.

Built for OSINT researchers who don't read Chinese fluently, to build muscle memory with the interaction mechanics before encountering them in the field.

## What's in here

- **Thirteen practice modules**, grouped by whether the challenge is genuinely China-specific (requires reading Chinese), Chinese-inflected (a universal mechanic with Chinese rendering or a Chinese-vendor product), or a global mechanic Chinese vendors adopted rather than invented.
- **Difficulty toggle** — Clean / Light distortion / Realistic. Realistic mode scatters glyphs over a procedurally generated backdrop with rotation, skew, and occasional flips, matching how live widgets actually render.
- **Vendor attribution** for every module — which Chinese companies (GeeTest, NetEase Yidun, Tencent, Dingxiang, Ishumei, Alibaba Cloud) ship that exact type, where known.
- **An open-access research citation** for every module, with a DOI and a working free-PDF link.

No build step, no dependencies, no external network calls. Backgrounds are generated on a `<canvas>` at runtime with a seeded PRNG — nothing is fetched or embedded from live CAPTCHA vendors.

## Running it locally

Just open `index.html` in a browser. Nothing to install.

## Deployment

Hosted as a static site. See the project's deployment notes for the current setup.

## Corrections welcome

Several of the vendor and citation mappings here were corrected mid-development after review — particularly around which types are genuinely China-specific versus globally adopted, and which citation actually matches which mechanic. If you spot something wrong, please open an issue or a PR. Two modules (word-order click, word-group selection) still lack a paper studying them directly; if you know of one, that's an especially welcome correction.

## Credits

Built by Eve C. with Claude (Anthropic).

## License

MIT — see [LICENSE](LICENSE).
