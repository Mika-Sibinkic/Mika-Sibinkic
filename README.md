# Mika Sibinkic

Founder of [Null Systems](https://nullsystemsllc.com), an applied-AI consultancy. I go into a company, find the workflow that costs the most time or money, and build the system that removes it. Discovery through production, then I hand it off and keep it running.

Most of my code is private. Every production system below was built for a client and lives in their repo or mine under an agreement that keeps it that way. The contribution graph is real; the repos behind it are not public. What I can show is below, and I will walk through any of the private codebases on a call.

## What I have shipped

| System | Client | What it does | Stack |
|---|---|---|---|
| AI Sourcing Specialist | Paychex, global talent acquisition | Recruiter uploads a job description; candidates are sourced, ranked, contacted, and interviews are scheduled. Private LLM outputs, orchestrated agents, hybrid BM25 + vector retrieval with a reranking feedback loop. | Python, PostgreSQL + pgvector, Google ADK, OpenAI API, iCIMS and LinkedIn integrations |
| Contact Extractor | JetLoan Capital, aviation lending | Broker emails forwarded to one inbox are parsed, validated, enriched, and upserted into Zoho CRM. Email content never leaves the firm's network. Runs on on-prem hardware I specced and set up. | n8n, Ollama, Docker, Windows on-prem |
| Funding Source Database | JetLoan Capital | Custom CRM for one contact type out of 22, driving high-stakes internal decisions. Deterministic parsing and routing around a small set of local models. In production, CI-gated. | Next.js, TypeScript, Vercel, Postgres + pgvector |
| Aperture | Cul2vate, Tennessee food-donation nonprofit | One tap on an old iPad logs a donation batch: camera captures it, a vision model estimates weight from learned density priors, the record lands in the sheet. Earned the client additional state subsidy. | Python, FastAPI, OpenCV, YOLOv8, ChArUco calibration, Cloudflare Tunnel, Next.js PWA |
| MicroScout | Nashville record label (undisclosed) | Label enters an artist and a budget. Micro-influencers are discovered, scored, contacted, negotiated with, contracted, paid, and measured through a nine-stage agentic pipeline with money-safety invariants at the database level and a human checkpoint at every consequential step. | Next.js, TypeScript, Supabase with RLS, Stripe Connect, Resend, Apify, 75 test suites in CI |

## What is public

- **[null-systems-nsos](https://github.com/Mika-Sibinkic/null-systems-nsos)**: my own diagnostic engine. Six parallel agent teams run question batteries against a company's data snapshot, reconcile findings, and produce a CEO-language opportunity report. Internal prototype, runs end to end on a synthetic client, tests in CI.
- **[ai-delivery-playbook](https://github.com/Mika-Sibinkic/ai-delivery-playbook)**: the rules I run AI coding agents under on client work. Verification ladder, decision tiers, secrets discipline, when an agent may act alone and when it stops. Written and revised over months of real deployments; failure modes in it were measured from session transcripts, not imagined.

## How I work with AI

I build with coding agents in the loop and I do not hide it. Commits in my repos carry co-author trailers when an agent wrote the diff. The part that matters is what sits around the agent: a written spec before the run, a stated stopping condition, tests that run from a clean clone, a decision record for anything architectural, and a four-rung status ladder where "tests pass" is the bottom rung and "the client saw it working" is the top. The playbook above is that system.

## Elsewhere

- [nullsystemsllc.com](https://nullsystemsllc.com)
- [LinkedIn](https://linkedin.com/in/mika-sibinkic)
- mikasibinkic@gmail.com

B.B.A. Finance and Economics, Belmont University, class of 2027.
