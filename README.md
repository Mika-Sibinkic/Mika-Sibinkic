# Mika Sibinkic

Founder of [Null Systems](https://nullsystemsllc.com), an applied-AI consultancy. I go into a company, find the workflow(s) that costs the most time or money, and build the system that flips it completely upside down. My team and I handle discovery all the way through production, then I hand it off and keep it running after some iterating per clients' needs.

Most of this work was built for clients and three of those repos are public below this with client data stripped out and disclosures respected. Sadly, the rest will have to stay private under agreements of mine.

## What I have shipped

| System | Client | What it does | Stack |
|---|---|---|---|
| AI Sourcing Specialist | Paychex, global talent acquisition | Recruiter uploads a job description; candidates are sourced, ranked, contacted, and interviews are scheduled. Private LLM outputs, orchestrated agents, hybrid BM25 + vector retrieval with a reranking feedback loop. | Python, PostgreSQL + pgvector, Google ADK, OpenAI API, iCIMS and LinkedIn integrations |
| Contact Extractor | JetLoan Capital, aviation lending | Broker emails forwarded to one inbox are parsed, validated, enriched, and upserted into Zoho CRM. Email content never leaves the firm's network. Runs on on-prem hardware I specced and set up. | n8n, Ollama, Docker, Windows on-prem |
| Funding Source Database | JetLoan Capital | Custom CRM for one contact type out of 22, driving high-stakes internal decisions. Deterministic parsing and routing around a small set of local models. In production, CI-gated. | Next.js, TypeScript, Vercel, Postgres + pgvector |
| Aperture | Cul2vate, Tennessee food-donation nonprofit | One tap on an old iPad logs a donation batch: camera captures it, a vision model estimates weight from learned density priors, the record lands in the sheet. Earned the client additional state subsidy and aided in a 1st place national victory for the Enactus team. | Python, FastAPI, OpenCV, YOLOv8, ChArUco calibration, Cloudflare Tunnel, Next.js PWA |
| MicroScout | Nashville record label (undisclosed) | Label enters an artist and a budget, and then micro-influencers are discovered, scored, contacted, negotiated with, contracted, paid, and measured through a nine-stage agentic pipeline with money-safety invariants at the database level and a human checkpoint at every consequential step. | Next.js, TypeScript, Supabase with RLS, Stripe Connect, Resend, Apify, 75 test suites in CI |

## How I work with AI

I build with coding agents in the loop and I do not hide it is for sure. Commits in my repos pretty much always co-author trailers when an agent wrote the diff. But, I always ensure a written spec before the run, a stated set of stopping conditions and rails, tests that run from clean clones, decision records for literally anything architectural, usually a four-rung status ladder where "tests pass" is the bottom rung and I have "the client saw it working" as the top, among other methods.

## Elsewhere

- [nullsystemsllc.com](https://nullsystemsllc.com)
- [LinkedIn](https://linkedin.com/in/mika-sibinkic)
- mikasibinkic@gmail.com


Thanks for visiting! XD
