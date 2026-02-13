# Mistral AI Worldwide Hackathon 2026 — Winning Strategy & Submission Plan

**Task ID:** `o65MQ3sGnEu3antKUycrO`  
**Goal:** execution-ready plan for Feb 28–Mar 1, 2026 using existing office assets (liquidation prevention + AI agent tooling).

---

## 1) Rules/Deadline Verification (with sources)

## Verified facts
- **Dates:** **Feb 28 – Mar 1, 2026** (48 hours).  
  Source: https://worldwide-hackathon.mistral.ai/
- **Format:** 7 cities + **online** participation.  
  Source: https://worldwide-hackathon.mistral.ai/
- **Team size:** **1–4 people**.  
  Source: https://worldwide-hackathon.mistral.ai/ and city pages (example London): https://luma.com/mistralhack-london
- **Prize headline:** **$200K+ total prizes**.  
  Source: https://worldwide-hackathon.mistral.ai/
- **Global winner:** **$10,000 cash + $15,000 Mistral credits + hiring opportunity**.  
  Source: https://worldwide-hackathon.mistral.ai/
- **Per-location prizes:** 1st ($1,500 + $3,000 credits), 2nd ($1,000 + $2,000 credits), 3rd ($500 + credits).  
  Source: https://worldwide-hackathon.mistral.ai/ and https://luma.com/mistralhack-london
- **Special awards (global/sponsor):** Best Vibe usage, Best use of ElevenLabs, Best video game project, Best use of agent skills.  
  Source: https://worldwide-hackathon.mistral.ai/
- **Sponsors mentioned:** W&B, NVIDIA, AWS, Hugging Face, ElevenLabs, Supercell (+ regional sponsors).  
  Source: https://worldwide-hackathon.mistral.ai/

## Operational note (must verify during briefing)
- Exact submission portal/mechanics (Devpost/form) are **not fully specified on public landing page**. The official briefing is listed for **Feb 25**.  
  Source: schedule on https://worldwide-hackathon.mistral.ai/

---

## 2) Best Prize-Track Selection Matrix (ranked by win probability)

| Rank | Track / Prize Bucket | Fit to Existing Assets | Build Effort | Estimated Win Probability* | Why this rank |
|---|---|---|---|---|---|
| 1 | **Best Use of Agent Skills** (special award) | **Very high** (already have AI agent + liquidation monitoring logic) | Medium | **High** | Directly aligned with our current code strengths; easiest differentiation via agent behavior and tooling depth. |
| 2 | **Local Podium (1st/2nd/3rd)** | High | Medium | Medium-High | 48h hackathons reward clean demos + reliability; we can ship a polished, practical product fast. |
| 3 | **Global Winner** | Medium-High | High | Medium-Low | Strong upside, but highest competition and requires exceptional novelty + presentation polish. |
| 4 | **Best Vibe Usage** | Medium | Medium | Medium | Depends on quality of integration with Mistral “Vibe” capabilities and visible UX impact. |
| 5 | **Best use of ElevenLabs** | Medium | Medium | Medium-Low | Adds scope (voice pipeline) and can distract from core alpha unless tightly scoped. |
| 6 | **Best Video Game Project** | Low | High | Low | Weak fit for our current repo assets; avoid for this cycle. |

\*Relative probability estimate for internal prioritization only.

**Recommendation:** Optimize for **Agent Skills + Local Podium** first, then position the same project narrative for Global Winner.

---

## 3) Project Concepts Leveraging Existing Assets

## Primary concept (recommended)
## **RiskPilot-M — Mistral Agent for DeFi Liquidation Prevention**

**What it is:** An agentic risk copilot that monitors lending positions (Kamino/MarginFi/Solend-style adapters), explains liquidation risk in plain English, and proposes/executes mitigation actions with human approval gates.

**Reuse from existing office assets:**
- Existing liquidation-prevention backend/logic patterns
- Existing multi-protocol adapter approach
- Existing MCP-style developer tooling direction

**Mistral-specific value:**
- Use Mistral models for risk summarization, next-best-action generation, scenario simulation prompts, and alert narratives.
- Optional: structured tool-calling style for deterministic action plans.

**Why judges care:** Real-world pain point + measurable outcome (reduced liquidation events, faster response).

## Backup concept (if DeFi data/API risk blocks primary)
## **IncidentPilot-M — On-call Incident Triage Agent for Dev Teams**

**What it is:** Mistral-powered agent that ingests logs/alerts, clusters incidents, proposes runbook steps, and drafts status updates.

**Reuse from existing assets:**
- Existing agent orchestration patterns
- Existing dashboard and alerting UX scaffolding

**Why this backup:** Keeps “agent skills” strength while removing on-chain/API volatility risk.

---

## 4) Required Submission Checklist (execution-ready)

## A. Code & Repo
- [ ] Public GitHub repo (clean README, setup, architecture, license)
- [ ] `uv`-based Python setup (`uv sync`, `uv run ...`)
- [ ] Reproducible `.env.example`
- [ ] No dead links, no placeholder demo URLs

## B. Demo
- [ ] Live demo URL (or local run steps if allowed by rules)
- [ ] 2–3 minute demo video (unlisted YouTube)
- [ ] Script shows: problem → agent action → measurable outcome

## C. Submission Content
- [ ] 200–400 word concise writeup
- [ ] Architecture diagram (PNG/SVG + README embed)
- [ ] 3–5 screenshots/GIFs with captions
- [ ] “Built with” list explicitly includes Mistral stack

## D. Compliance/Quality
- [ ] Team size ≤ 4 confirmed
- [ ] Build window compliance (new work during event)
- [ ] Explicitly disclose any pre-existing code reused
- [ ] Rebrand all prior hackathon references in UI/README

---

## 5) 10-Day Sprint Plan (owners + milestones)

Assume **D-10 = now**, **D0 = hackathon start**.

| Day | Owner | Milestone | Exit Criteria |
|---|---|---|---|
| D-10 | Henry + PM | Lock primary + backup scope | One-page scope freeze, success metric chosen |
| D-9 | Dev Lead | Repo hardening + baseline runbook | Clean install/run on fresh machine |
| D-8 | Agent Eng | Mistral integration spike | Working prompt/tool loop demo |
| D-7 | Data/Backend | Protocol adapter stabilization | Risk score + health-factor outputs stable |
| D-6 | Frontend | Demo UI pass | Core flows clickable with realistic data |
| D-5 | QA | Reliability + failure-mode testing | Known error paths handled, no hard crashes |
| D-4 | Content | Draft Devpost writeup + architecture diagram | First complete submission draft |
| D-3 | Demo Owner | Record v1 demo video | 2–3 min watchable cut |
| D-2 | Team | Judge simulation + polish | 2 mock judge Q&A rounds complete |
| D-1 | Team | Final packaging + freeze | Final repo tag + final links ready |
| D0/D1 | Team | Hackathon execution window | Submit on-time with all artifacts |

---

## 6) Risk Register + Mitigation

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| Submission mechanics change late | Medium | High | Attend Feb 25 briefing; keep checklist modular; assign one owner to rules watch. |
| API instability / model limits | Medium | High | Pre-cache fallback responses; maintain a degraded local/mock mode. |
| Over-scoping during 48h | High | High | Strict MVP gate: one killer flow > many half-features. |
| DeFi data dependency outages | Medium | Medium-High | Backup concept (IncidentPilot-M) ready by D-5. |
| Demo failure (latency/network) | Medium | High | Record deterministic backup video + local fallback demo script. |
| Judges don’t grasp value quickly | Medium | High | First 20 seconds: “who/what/value” + one concrete before/after metric. |

---

## Final Recommendation (do this now)
1. **Commit to Primary:** RiskPilot-M (Agent Skills + Local Podium focus).  
2. **Use backup only if blocked by D-5:** switch to IncidentPilot-M.  
3. **Optimize for judging:** reliable end-to-end demo, explicit Mistral usage, measurable impact metric, clean submission artifacts.

---

## Quick Sources
- Official worldwide page: https://worldwide-hackathon.mistral.ai/
- London city page (practical details): https://luma.com/mistralhack-london
- Paris city page (cross-check): https://luma.com/mistralhack-paris
