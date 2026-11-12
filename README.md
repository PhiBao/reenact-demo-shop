# Corner Shop: a demo target for Reenact

A tiny coffee-gear store (a cart, quantities, a coupon box) used to show [Reenact](https://github.com/PhiBao/reenact) end to end on GitHub Actions.

**Its bugs were planted by the Reenact authors** so that there is something to reproduce and fix. They are not claims about real software; the claims about real apps are in the Reenact repo (Memos benchmarks and two real fixes).

What to look at:

- [Issue #1](https://github.com/PhiBao/reenact-demo-shop/issues/1): a messy report becomes a browser reproduction with screenshots, then `/reenact fix` opens [PR #2](https://github.com/PhiBao/reenact-demo-shop/pull/2).
- [Issue #5](https://github.com/PhiBao/reenact-demo-shop/issues/5): "checkout is broken" gets *Needs info*, the reporter answers, Reenact reproduces it, fixes it and re-runs three earlier tests ([PR #8](https://github.com/PhiBao/reenact-demo-shop/pull/8)).
- [`reenact/tests/`](reenact/tests): the plain-English tests Reenact keeps. `reenact suite` re-runs them live.
- [`.github/workflows/reenact.yml`](.github/workflows/reenact.yml): the whole integration. Issue text is untrusted, so it only auto-runs for people with write access; anyone else needs a maintainer to add the `reenact` label.

Run it: `node server.js` (port 4100).
