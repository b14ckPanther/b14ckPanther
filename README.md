<div align="center">

<a href="https://zangeel.dev"><img src="assets/hero.svg" width="100%" alt="Nour Alden Mousa, founder and engineer of Darb. Full-stack and mobile software engineer building the search, maps and apps that connect people to local businesses."/></a>

<br/><br/>

<a href="https://zangeel.dev"><img src="https://img.shields.io/badge/Portfolio-zangeel.dev-d9a54c?style=for-the-badge&labelColor=0e3527" alt="Portfolio: zangeel.dev"/></a>
<a href="https://darb.co.il/en"><img src="https://img.shields.io/badge/Darb-darb.co.il-f0c77a?style=for-the-badge&labelColor=0e3527" alt="Darb: darb.co.il"/></a>
<a href="https://www.linkedin.com/in/nmprofessor/"><img src="https://img.shields.io/badge/LinkedIn-nmprofessor-1d5a43?style=for-the-badge&logo=linkedin&logoColor=fbf7ec&labelColor=0e3527" alt="LinkedIn"/></a>
<a href="mailto:founder@darb.co.il"><img src="https://img.shields.io/badge/Email-founder@darb.co.il-1d5a43?style=for-the-badge&logo=maildotru&logoColor=fbf7ec&labelColor=0e3527" alt="Email founder@darb.co.il"/></a>

</div>

<br/>

## Darb

*Darb* means *path* in Arabic. It's what I'm building full time with my co-founder Lama: one path to every local business, and one platform that connects the people searching, the people adding businesses, and the businesses themselves.

It covers the north of Israel today. The goal is every city, town and village in the country, and to expand beyond it from there.

<a href="https://darb.co.il/en"><img src="assets/darb.svg" width="100%" alt="Darb search: a request in plain words is read as what, where and must-have. 13,000+ real businesses across 1,138 places and 211 kinds of business, about 1,500 tests on every pull request."/></a>

<br/>

<img src="assets/darb-paths.svg" width="100%" alt="One platform with paths to every app: Darb, Darb Helpers and Darb Admin on one side; Darb REST, YellowShifts, Caramel and Raghad Beauty on the other."/>

**How it's built**

- **Its own backend, built from zero.** No backend-as-a-service: a NestJS API we wrote ourselves for search, places, media, admin, helpers and pricing, on our own PostgreSQL schema with PostGIS and pgvector, Redis for caching and rate limits, and one set of shared zod contracts so a mismatched field between API and web fails the build, not production. The only outside service in the core is Clerk for sign-in.
- **Two-lane search.** An instant index answers in the browser as you type. A language model then reads the intent under a strict schema and a 1.5 s budget, and matches it against what each business offers, down to single menu items. If the model is slow, the instant results stand on their own.
- **One continuous map.** Country, town, category and business are levels of one camera on MapLibre GL, with self-hosted vector tiles on Cloudflare R2, so there's no per-view map bill and no third-party tracking.
- **Real data with sources.** Listings come from government registers and OpenStreetMap, deduplicated and geocoded. Darb Helpers and the admin's street capture fill in the towns the open maps miss, and every addition is reviewed before it goes live.
- **Nothing ships on a red build.** Type checks, about 1,500 unit and integration tests against a real database, Playwright on desktop and phone, WCAG AA checks on every page, per-route performance budgets and a 103-query search quality set run on every pull request.

<sub>Next.js 16 · NestJS · Prisma · PostgreSQL with PostGIS and pgvector · Redis · MapLibre GL · Cloudflare R2 · Railway · Vercel · Turborepo</sub>

<a href="https://darb.co.il/en"><img src="https://img.shields.io/badge/Open_Darb-darb.co.il-d9a54c?style=flat-square&labelColor=0e3527" alt="Open Darb"/></a>
<a href="https://github.com/b14ckPanther/Darb-City"><img src="https://img.shields.io/badge/Source-Darb--City-1d5a43?style=flat-square&logo=github&logoColor=fbf7ec&labelColor=0e3527" alt="Darb-City source"/></a>

<br/>

## More work

<p>
<a href="https://paz.darb.co.il"><img src="assets/projects/yellowshifts.svg" width="49%" alt="YellowShifts: shift scheduling and NFC attendance for fuel stations, in pilot at a working Paz station."/></a>
<a href="https://rest.darb.co.il"><img src="assets/projects/darb-rest.svg" width="49%" alt="Darb REST: digital menus and WhatsApp ordering for restaurants and cafés, run by the owners."/></a>
</p>
<p>
<a href="https://caramel.darb.co.il"><img src="assets/projects/caramel.svg" width="49%" alt="Caramel: a menu where caramel pours down the page and wraps each dish. Built with Lama."/></a>
<a href="https://zangeel.dev"><img src="assets/projects/nours-world.svg" width="49%" alt="Nour's World: a playable 3D portfolio. Drive an island where every landmark is a product."/></a>
</p>

<sub>Source: [PazShifts](https://github.com/b14ckPanther/PazShifts) (YellowShifts), [Darb_Rest](https://github.com/b14ckPanther/Darb_Rest), [Caramel](https://github.com/Lzbedat3/Caramel_next) on Lama's profile, [Nour's World](https://github.com/b14ckPanther/Nours-World) (public showcase).</sub>

<br/>

## Toolbox

| | |
| :-- | :-- |
| **Languages** | <img src="https://skillicons.dev/icons?i=ts,js,java,c,dart,py&theme=dark" height="40" alt="TypeScript, JavaScript, Java, C, Dart, Python"/> |
| **Web** | <img src="https://skillicons.dev/icons?i=nextjs,react,tailwind,threejs&theme=dark" height="40" alt="Next.js, React, Tailwind CSS, Three.js"/> |
| **Mobile** | <img src="https://skillicons.dev/icons?i=flutter,react&theme=dark" height="40" alt="Flutter, React Native"/><br/><sub>Flutter, React Native with Expo</sub> |
| **Backend** | <img src="https://skillicons.dev/icons?i=nodejs,nestjs,prisma,supabase&theme=dark" height="40" alt="Node.js, NestJS, Prisma, Supabase"/> |
| **Data** | <img src="https://skillicons.dev/icons?i=postgres,redis,mysql&theme=dark" height="40" alt="PostgreSQL, Redis, MySQL"/> |
| **Ship** | <img src="https://skillicons.dev/icons?i=vercel,cloudflare,docker,githubactions,linux,figma&theme=dark" height="40" alt="Vercel, Cloudflare, Docker, GitHub Actions, Linux, Figma"/> |

<br/>

## Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/b14ckPanther/b14ckPanther/output/snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/b14ckPanther/b14ckPanther/output/snake-light.svg"/>
  <img src="https://raw.githubusercontent.com/b14ckPanther/b14ckPanther/output/snake-dark.svg" width="100%" alt="Contribution graph eaten by a gold snake"/>
</picture>

<br/>

## Get in touch

I'm happy to talk about Darb, partnerships, local business tech, or engineering work. Email [founder@darb.co.il](mailto:founder@darb.co.il), find me on [LinkedIn](https://www.linkedin.com/in/nmprofessor/), or drive around [zangeel.dev](https://zangeel.dev).

<br/>

<div align="center">
<sub>© 2026 Nour Alden Mousa</sub>
</div>
