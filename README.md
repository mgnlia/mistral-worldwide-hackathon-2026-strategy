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
- **Special awards (global/sponsor):** Best Vibe usage (AirPods), Best use of ElevenLabs ($2K credits/member), Best video game project (Game Boy), Best use of agent skills (**Custom Reachy Mini robot — physical, non-cash**).  
  Source: https://worldwide-hackathon.mistral.ai/
- **Sponsors mentioned:** W&B, NVIDIA, AWS, Hugging Face, ElevenLabs, Supercell (+ regional sponsors).  
  Source: https://worldwide-hackathon.mistral.ai/

## Operational note (must verify during briefing)
- Exact submission portal/mechanics (Devpost/form) are **not fully specified on public landing page**. The official briefing is listed for **Feb 25**.  
  Source: schedule on https://worldwide-hackathon.mistral.ai/

---

## 2) Best Prize-Track Selection Matrix (ranked by win probability)

> ⚠️ **CORRECTED Feb 2026 (adversary gate):** "Best Use of Agent Skills" prize is a **Custom Reachy Mini robot** (physical hardware, non-cash). It was previously ranked #1 under a mistaken assumption of cash value. Primary cash targets are Global Winner and Online Podium. Matrix updated accordingly.

| Rank | Track / Prize Bucket | Prize Value | Fit to Existing Assets | Build Effort | Estimated Win Probability* | Why this rank |
|---|---|---|---|---|---|---|
| 1 | **Global Winner** | $10,000 cash + $15,000 credits + hiring | Medium-High | High | Medium-Low | Highest cash value; requires exceptional novelty + polish; worth targeting with same build |
| 2 | **Online Podium 1st** | $1,500 cash + $3,000 credits | High | Medium | Medium-High | 48h hackathons reward clean demos + reliability; strong fit for our agent tooling |
| 3 | **Online Podium 2nd/3rd** | $1,000/$500 cash + credits | High | Medium | Medium-High | Same build path as 1st; floor protection if 1st is competitive |
| 4 | **Best Use of ElevenLabs** | $2,000/member in credits | Medium | Medium | Medium-Low | Adds voice scope; only pursue if it fits naturally into demo flow |
| 5 | **Best Use of Agent Skills** | Custom Reachy Mini robot (non-cash) | Very High | Medium | High | Strong fit, but prize is a physical robot — deprioritized vs. cash tracks |
| 6 | **Best Vibe Usage** | Branded AirPods (non-cash) | Medium | Medium | Medium | Non-cash; only if Mistral Vibe integration is natural |
| 7 | **Best Video Game Project** | Game Boy + Supercell consideration | Low | High | Low | Weak fit; avoid |

\*Relative probability estimate for internal prioritization only.

**Recommendation:** Optimize for **Global Winner + Online Podium** (cash) first. Agent Skills (robot) is a natural byproduct of the same build — do not deprioritize the code quality for it, but do not optimize toward it over cash prizes.

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

**Status:** Baseline scaffold live at https://github.com/mgnlia/riskpilot-m — uv-based, Mistral API integrated, tool-calling spike functional.

## Backup concept (if DeFi data/API risk blocks primary)
## **IncidentPilot-M — On-call Incident Triage Agent for Dev Teams**

**What it is:** Mistral-powered agent that ingests logs/alerts, clusters incidents, proposes runbook steps, and drafts status updates.

**Reuse from existing assets:**
- Existing agent orchestration patterns
- Existing dashboard and alerting UX scaffolding

**Why this backup:** Keeps "agent skills" strength while removing on-chain/API volatility risk.

---

## 4) Required Submission Checklist (execution-ready)

## A. Code & Repo
- [x] Public GitHub repo (clean README, setup, architecture, license) — https://github.com/mgnlia/riskpilot-m
- [x] `uv`-based Python setup (`uv sync`, `uv run ...`)
- [x] Reproducible `.env.example`
- [ ] No dead links, no placeholder demo URLs

## B. Demo
- [ ] Live demo URL (or local run steps if allowed by rules)
- [ ] 2–3 minute demo video (unlisted YouTube)
- [ ] Script shows: problem → agent action → measurable outcome

## C. Submission Content
- [ ] 200–400 word concise writeup
- [ ] Architecture diagram (PNG/SVG + README embed)
- [ ] 3–5 screenshots/GIFs with captions
- [ ] "Built with" list explicitly includes Mistral stack

## D. Compliance/Quality
- [ ] Team size ≤ 4 confirmed
- [ ] Build window compliance (new work during event)
- [ ] Explicitly disclose any pre-existing code reused
- [ ] Rebrand all prior hackathon references in UI/README

---

## 5) Sprint Plan (updated to reflect current state)

Hackathon starts Feb 28. Today ~Feb 20. ~8 days remain.

| Milestone | Owner | Status | Exit Criteria |
|---|---|---|---|
| Repo + baseline spike | Dev/Sage | ✅ DONE | riskpilot-m live, basic + tool-loop modes working |
| Strategy doc corrected | Adversary gate | ✅ DONE | Prize matrix updated (this commit) |
| **Registration proof** | **HUMAN** | ❌ **BLOCKING** | Screenshot/URL of Luma wallet verification posted in task |
| Protocol adapter (D-7) | Dev | ❌ Not started | Health-factor scoring with mock on-chain data |
| Demo UI (D-6) | Dev | ❌ Not started | Streamlit or rich-CLI showing risk score + next action |
| QA / failure modes (D-5) | Dev | ❌ Not started | No hard crashes on bad input |
| Submission writeup + diagram (D-4) | Sage | ❌ Not started | Draft writeup + architecture diagram in README |
| Demo video v1 (D-3) | Human | ❌ Not started | 2–3 min watchable cut uploaded to YouTube |
| Judge simulation + polish (D-2) | Team | ❌ Not started | 2 mock Q&A rounds complete |
| Final freeze (D-1) | Team | ❌ Not started | Final repo tag + all links ready |
| Hackathon execution (D0/D1) | Team | — | Submit on-time |

---

## 6) Risk Register + Mitigation

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| **Registration not approved** | **High** | **Critical** | **Human must submit wallet verification at https://luma.com/mistralhack-online TODAY. Confirmation window closes ~Feb 21.** |
| Submission mechanics change late | Medium | High | Attend Feb 25 briefing; keep checklist modular; assign one owner to rules watch. |
| API instability / model limits | Medium | High | Pre-cache fallback responses; maintain a degraded local/mock mode. |
| Over-scoping during 48h | High | High | Strict MVP gate: one killer flow > many half-features. |
| DeFi data dependency outages | Medium | Medium-High | Backup concept (IncidentPilot-M) ready by D-5. |
| Demo failure (latency/network) | Medium | High | Record deterministic backup video + local fallback demo script. |
| Judges don't grasp value quickly | Medium | High | First 20 seconds: "who/what/value" + one concrete before/after metric. |

---

## Final Recommendation
1. **IMMEDIATE:** Human operator submits Luma registration + wallet verification.  
2. **Cash targets:** Global Winner + Online Podium (not Agent Skills robot).  
3. **Next code milestone:** Protocol adapter with health-factor scoring (D-7).  
4. **Optimize for judging:** reliable end-to-end demo, explicit Mistral usage, measurable impact metric, clean submission artifacts.

---

## Quick Sources
- Official worldwide page: https://worldwide-hackathon.mistral.ai/
- Online registration: https://luma.com/mistralhack-online
- London city page (practical details): https://luma.com/mistralhack-london
- Paris city page (cross-check): https://luma.com/mistralhack-paris
- RiskPilot-M repo: https://github.com/mgnlia/riskpilot-m
