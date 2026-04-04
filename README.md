# Free for Dev

> A curated directory of **always-free** developer and DevOps services. No trials, no expiring credits — just genuinely free tiers you can rely on long-term.

**🔗 Live Site: [free-for-dev](https://girishlade111.github.io/free-for-dev/)**

---

## What Is This?

A single-page, zero-dependency directory of **159 free-tier services** across **22 categories**. Built for developers, indie hackers, and startups who want to build and ship without paying for infrastructure.

Every entry is verified against official free-tier documentation. Services are marked as **Always Free** or **Trial/Credit** so you know exactly what you're getting.

---

## Quick Stats

| Metric | Count |
|--------|-------|
| Total Services | **159** |
| Categories | **22** |
| Always-Free Services | **~140+** |
| External Dependencies | **0** |
| File Size | **~55 KB** |

---

## Categories

### ☁️ Major Cloud Providers
Full cloud platforms with always-free tiers: Oracle Cloud (4 ARM VMs, 200GB), Google Cloud (e2-micro, Cloud Run), Azure (40+ free services), IBM Cloud (25+ Lite services), and more.

### 🚀 Hosting & Deployment
Static and serverless hosting: Vercel, Netlify, Cloudflare Pages, GitHub Pages, Render, Fly.io, Deno Deploy, Surge, Glitch, Koyeb, PythonAnywhere.

### 🔄 CI/CD & Automation
Build and deploy pipelines: GitHub Actions (2000 min/mo, unlimited for public), GitLab CI, CircleCI, Azure DevOps, Travis CI, Drone CI, Woodpecker CI, Semaphore CI, Jenkins.

### 🗄️ Databases (SQL & NoSQL)
Managed databases: Neon (PostgreSQL), Supabase (PostgreSQL), MongoDB Atlas, Redis Cloud, CockroachDB, TiDB, Turso (SQLite), Xata, Upstash (Redis/Kafka), InfluxDB, Fauna, DynamoDB, Appwrite, PocketBase.

### 💾 Storage & File Services
Object and file storage: Cloudflare R2 (10GB, no egress fees), Backblaze B2, Firebase Storage, Supabase Storage, Pinata (IPFS), Filebase.

### 🌐 DNS & Networking
DNS and tunneling: Cloudflare DNS (unlimited), Cloudflare Tunnels, DuckDNS, ngrok, localtunnel, Hurricane Electric DNS.

### ⚡ CDN & Edge Computing
Content delivery and edge compute: Cloudflare CDN (unlimited bandwidth), Cloudflare Workers, Vercel Edge Functions, Deno Deploy, AWS CloudFront.

### 📊 Monitoring & Logging
Infrastructure monitoring: Grafana Cloud, Datadog, Sentry, SigNoz, Better Stack, UptimeRobot, Healthchecks.io, OpenObserve, Axiom, Logtail.

### 🔐 Authentication & Identity
User auth and identity: Clerk (10K MAU), Supabase Auth, Firebase Auth, Auth0, Keycloak, Ory Kratos, SuperTokens, Zitadel.

### 💬 Messaging, Queues & Realtime
Realtime communication: Pusher Channels, Ably, PubNub, CloudAMQP, Upstash Kafka, RabbitMQ, NATS, Socket.io, Mercure.

### ✉️ Email & Transactional Mail
Email delivery: Resend (3K/mo), Brevo (300/day), AWS SES (3K/mo), Postmark (100/mo), Plunk (5K/mo), SendGrid (100/day).

### ⚙️ Serverless & Edge Functions
Function-as-a-service: AWS Lambda (1M req/mo), Cloudflare Workers, Vercel Serverless Functions, Netlify Functions, Google Cloud Functions, Deno Deploy, Azure Functions.

### 🔌 API Gateways & Management
API management: Kong Gateway, Tyk, Apache APISIX, Zuplo.

### 🚩 Feature Flags & Config
Feature flagging: Unleash, Flagsmith, ConfigCat, Hypertune.

### 📈 Analytics & Telemetry
Product analytics: Plausible, Umami, PostHog (1M events/mo), Mixpanel, Google Analytics, Fathom, GoatCounter.

### 🧪 Testing & QA
Browser testing: Playwright, Cypress Cloud, Lambdatest, Responsively. Free for open source: BrowserStack, Sauce Labs.

### 📝 Logging & Error Tracking
Error monitoring: Sentry, LogRocket, Highlight, Bugsnag, Rollbar.

### 📰 CMS & Headless
Content management: Strapi, Sanity, Contentful, Directus, Payload CMS, Ghost, Decap CMS.

### 🐳 Container Registry & Orchestration
Container hosting: Docker Hub, GitHub Container Registry, Quay.io, GitLab Container Registry.

### 🛠️ Developer Tools & APIs
Dev utilities: ngrok, Beeceptor, Webhook.site, Pipedream, n8n, StackBlitz, Replit, GitPod, MockAPI, JSON Server, SwaggerHub.

### 🛡️ Security & Secrets
Vulnerability scanning and secrets: Snyk, Dependabot, Trivy, HashiCorp Vault, Doppler, Akeyless.

### 🖼️ Image & Video
Media processing: Cloudinary (25K transformations/mo), ImageKit, Uploadcare, Mux.

---

## Features

### For Users
- **⚡ Fast & Lightweight** — Single HTML file, ~55 KB, zero external dependencies, works offline
- **🌓 Dark / Light Theme** — Toggle with preference saved to localStorage
- **🔍 Instant Search** — Filter services by name, category, or features (`/` to focus, `Escape` to clear)
- **📱 Mobile-Responsive** — Card-style layout on small screens, readable everywhere
- **🏷️ Clear Badges** — "Always Free" and "Trial/Credit" labels at a glance
- **📊 Stats Bar** — Total services, categories, and always-free count at the top
- **🖨️ Print-Friendly** — Hides interactive elements when printing
- **🔗 Anchor Navigation** — Sticky table of contents links every section

### For Developers
- **Zero Build Step** — No npm, no bundler, no framework. Just open `index.html`
- **SEO Optimized** — Meta description, Open Graph, Twitter Card tags, semantic HTML
- **Accessible** — ARIA labels, keyboard navigation, focus management
- **Easy to Contribute** — All service data is a JavaScript array at the top of the `<script>` block

---

## Getting Started

### Local Use
Simply open `index.html` in your browser. No server required.

```bash
# Or serve it locally with any HTTP server
npx serve .
# or
python -m http.server 8080
```

### Deploy Anywhere
Drop `index.html` on any static host:
- **GitHub Pages** — Push to a repo, enable Pages in settings
- **Netlify** — Drag and drop the file at app.netlify.com/drop
- **Vercel** — `vercel deploy` from the directory
- **Cloudflare Pages** — Connect your repo, zero config

---

## Project Structure

```
free-for-dev/
├── index.html      # Single-file application (HTML + CSS + JS)
└── README.md       # This file
```

That's it. No `node_modules`, no `package.json`, no build output.

---

## Adding or Editing Services

All service data lives in the `categories` array inside the `<script>` tag in `index.html`.

### Service Entry Format
```javascript
{
  name: "Service Name",
  url: "https://official-url",
  freeTier: "Description of free tier limits",
  alwaysFree: true,    // true = always free, false = trial/credit
  tag: "Optional Tag"  // e.g., "PostgreSQL", "Redis", "SQLite"
}
```

### Adding a New Category
```javascript
{
  id: "unique-id",
  name: "Category Name",
  icon: "🔥",
  services: [
    // ... service entries
  ]
}
```

### Guidelines for Contributions
1. **Always Free preferred** — Prioritize services with ongoing free tiers, not time-limited trials
2. **Verify limits** — Check the official free-tier page before submitting
3. **One sentence descriptions** — Keep freeTier field concise and specific
4. **Include official URLs** — Link to the official service page, not a blog post
5. **Mark trials clearly** — Set `alwaysFree: false` for credit-based or trial-only offers

---

## Why This Exists

Most "free tier" lists mix genuinely free services with expired trials and marketing fluff. This project focuses on **signal over noise**:

- Every service is verified against official documentation
- Always-free services are clearly labeled vs. trial/credit offers
- Limits are specific (numbers, not vague claims)
- Self-hosted open-source options are included where relevant

It's the resource I wanted when starting a side project with zero budget.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | Semantic HTML5 |
| Styling | CSS Custom Properties, Flexbox, CSS Grid |
| Interactivity | Vanilla JavaScript (ES6+) |
| Dependencies | None |
| Build Tool | None |

---

## Browser Support

Works on all modern browsers (Chrome, Firefox, Safari, Edge). No polyfills or transpilation needed.

---

## License

This project is open for anyone to use, fork, or modify. Built for the developer community.

---

## Contributing

Found a service with outdated limits? Want to add a new category or service?

1. Open `index.html`
2. Find the `categories` array in the `<script>` section
3. Add or edit entries following the format above
4. Submit a Pull Request

---

**🔗 Bookmark this: [free-for-dev](https://girishlade111.github.io/free-for-dev/)**
