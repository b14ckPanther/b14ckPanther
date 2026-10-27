<div align="center">

<a href="https://zangeel.dev"><img src="assets/hero.svg" width="100%" alt="Nour Alden Mousa, full-stack and mobile software engineer, open to full-time roles. Builds products end to end, from the database and API to the interface. Founder of Darb, built from zero."/></a>

<br/><br/>

<a href="#get-in-touch"><img src="https://img.shields.io/badge/Open_to_work-Full--time_roles-f0c77a?style=for-the-badge&labelColor=0e3527" alt="Open to work: full-time roles"/></a>
<a href="https://zangeel.dev"><img src="https://img.shields.io/badge/Portfolio-zangeel.dev-d9a54c?style=for-the-badge&labelColor=0e3527" alt="Portfolio: zangeel.dev"/></a>
<a href="https://www.linkedin.com/in/nouraldenmousa/"><img src="https://img.shields.io/badge/LinkedIn-nouraldenmousa-1d5a43?style=for-the-badge&logo=linkedin&logoColor=fbf7ec&labelColor=0e3527" alt="LinkedIn"/></a>
<a href="mailto:founder@darb.co.il"><img src="https://img.shields.io/badge/Email-founder@darb.co.il-1d5a43?style=for-the-badge&logo=maildotru&logoColor=fbf7ec&labelColor=0e3527" alt="Email founder@darb.co.il"/></a>

</div>

<br/>

## Darb, my personal project

**Darb is my own product, not an employer's.** *Darb* means *path* in Arabic. I founded it with Lama, my co-founder, and engineered it from the ground up: one path to every local business, and one platform that connects the people searching, the people adding businesses, and the businesses themselves.

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

## Darb Lab

Darb Lab is where I build with the stacks Darb doesn't use: Java and Spring, C# and .NET, Python and machine learning. Each one is a product of its own, and they all share one world. Every Lab project sends its real events into **Darb Budokai**, an RPG powered by my real life.

<p>
<a href="https://github.com/b14ckPanther/darb-scouter"><img src="assets/projects/darb-scouter.svg" width="49%" alt="Darb Scouter: reads each new junior job in Israel at 07:00 and scores it against my CV, quote by quote. Working."/></a>
<a href="https://github.com/b14ckPanther/darb-budokai"><img src="assets/projects/darb-budokai.svg" width="49%" alt="Darb Budokai: the RPG my real life powers. Java 21, Spring Boot, Kafka and Angular. In build."/></a>
</p>
<p>
<a href="https://github.com/b14ckPanther/darb-sennin"><img src="assets/projects/darb-sennin.svg" width="49%" alt="Darb Sennin: code practice with an honest reviewer that shows the evidence behind every grade. C#, .NET 10 and MongoDB. In build."/></a>
<a href="https://github.com/b14ckPanther/darb-juryoku"><img src="assets/projects/darb-juryoku.svg" width="49%" alt="Darb Juryoku: a posture coach that runs in the browser with MediaPipe and a PyTorch model. Webcam frames never leave the device. In build."/></a>
</p>

<sub>Planned next: [Darb Capsule](https://github.com/b14ckPanther/darb-capsule) (Flutter companion with a live home-screen widget), [Darb Genki](https://github.com/b14ckPanther/darb-genki) (Budokai on Kubernetes, traced with OpenTelemetry), [Darb Ki](https://github.com/b14ckPanther/darb-ki) (AWS honeypots with ML attack sorting), [Darb Kinton](https://github.com/b14ckPanther/darb-kinton) (end-to-end encrypted transfer in Go).</sub>

<br/>

## Toolbox

| | |
| :-- | :-- |
| **Languages** | <img src="https://skillicons.dev/icons?i=ts,js,java,cs,py,dart,c&theme=dark" height="40" alt="TypeScript, JavaScript, Java, C#, Python, Dart, C"/> |
| **Web** | <img src="https://skillicons.dev/icons?i=nextjs,react,angular,tailwind,threejs&theme=dark" height="40" alt="Next.js, React, Angular, Tailwind CSS, Three.js"/> |
| **Mobile** | <img src="https://skillicons.dev/icons?i=flutter,react&theme=dark" height="40" alt="Flutter, React Native"/><br/><sub>Flutter, React Native with Expo</sub> |
| **Backend** | <img src="https://skillicons.dev/icons?i=nodejs,nestjs,spring,dotnet,fastapi,prisma,supabase&theme=dark" height="40" alt="Node.js, NestJS, Spring Boot, .NET, FastAPI, Prisma, Supabase"/> |
| **Data** | <img src="https://skillicons.dev/icons?i=postgres,redis,mongodb,elasticsearch,mysql&theme=dark" height="40" alt="PostgreSQL, Redis, MongoDB, Elasticsearch, MySQL"/> |
| **AI and ML** | <img src="https://skillicons.dev/icons?i=pytorch&theme=dark" height="40" alt="PyTorch"/><br/><sub>Claude API with structured outputs, LangGraph, MediaPipe, ONNX Runtime Web</sub> |
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

I'm looking for a full-time software engineering role: full-stack, frontend or mobile. I own features from the data model to the final UI, and Darb shows how I work at scale. Email [founder@darb.co.il](mailto:founder@darb.co.il), find me on [LinkedIn](https://www.linkedin.com/in/nouraldenmousa/), or drive around [zangeel.dev](https://zangeel.dev).

<br/>

<div align="center">
<sub>© 2026 Nour Alden Mousa</sub>
</div>
