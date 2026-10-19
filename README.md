# mattmcf.com

Personal index for [mattmcf.com](https://mattmcf.com): a static homepage linking to [MN Parks](https://parks.mattmcf.com), [LinkedIn](https://linkedin.mattmcf.com), and [GitHub](https://github.com/mattmcf). It is a map of the domain, not a geographic park map.

Hosted on **GitHub Pages** ($0) from this public repo. Parks stays on Render at `parks.mattmcf.com`. LinkedIn stays on the existing `linkedin` A records.

## Local

```bash
npm install
npm run dev
```

Dev server: [http://127.0.0.1:43123](http://127.0.0.1:43123).

```bash
npm run build
npm run preview
```

## GitHub Pages

Publishing source is **GitHub Actions** (`.github/workflows/pages.yml`): push to `main` builds the Vite site and deploys `dist/`. Custom domain: **`mattmcf.com`**.

Default Pages URL until DNS is live: [https://mattmcf.github.io/mattmcf.com/](https://mattmcf.github.io/mattmcf.com/).

Apex DNS must use GitHub Pages **A** records. Replace only the GoDaddy **WebsiteBuilder Site** `@` A record. Leave `parks`, `linkedin`, NS, SOA, TXT, and `_domainconnect` alone.
