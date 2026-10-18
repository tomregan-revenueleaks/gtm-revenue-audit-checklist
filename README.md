# GTM Revenue Audit Checklist
Built from hands-on B2B GTM audits.

A comprehensive checklist for auditing your B2B go-to-market motion and identifying revenue leaks.

## Overview

This checklist helps you systematically identify and quantify the revenue leaks in your GTM processes.

Built from hands-on audits across SaaS, FinTech, HealthTech and professional services.

## Quick Start

**Automated audit:** Artemis, the AI GTM Engineer, is a free installable agent that teams run in their own Claude Code, claude.ai or Codex. It runs a GTM audit in one session: [artemisgtm.ai/engineer](https://artemisgtm.ai/engineer/)

**Manual Audit:** Use the checklists below to systematically review your GTM motion.

---

## The Audit Framework

### 1. Lead Response Time

- [ ] Measure average time from form submission to first contact
- [ ] Benchmark: Under 5 minutes for high-intent (demo requests)
- [ ] Benchmark: Under 1 hour for medium-intent (content downloads)
- [ ] Calculate revenue impact of response delays

**Revenue Impact Formula:**

Monthly leads × Response rate delta × Conversion rate × Avg deal size = Annual leak
Example: 200 × 0.40 × 0.15 × 15,000 USD = 180,000 USD/year

### 2. Lead Routing

- [ ] Document current routing rules
- [ ] Verify rules match current territories/ownership
- [ ] Check if high-value leads get priority routing
- [ ] Audit round-robin fairness and availability logic
- [ ] Confirm no leads falling through cracks (unassigned)

**Red Flags:**
- Enterprise leads going to junior reps
- Routing rules older than 12 months
- No segment-based routing logic
- High volume of reassigned leads

### 3. MQL Definition & Handoff

- [ ] Written MQL definition exists
- [ ] Sales and marketing agree on MQL criteria
- [ ] SLA exists for MQL follow-up time
- [ ] Rejection reasons are required and tracked
- [ ] MQL rejection rate is under 15%

**Conversion Rate Starting Assumptions** (illustrative inputs; replace them with your own CRM numbers):
| Stage | Starting assumption |
|-------|-----------|
| Lead to MQL | 25-35% |
| MQL to SQL | 15-20% |
| SQL to Opportunity | 50-60% |
| Opportunity to Closed Won | 20-30% |

### 4. Pipeline Hygiene

- [ ] Deals have next steps scheduled
- [ ] Close dates are realistic (not all month-end)
- [ ] Stale deals are reviewed weekly
- [ ] Stage definitions are documented
- [ ] Required fields enforced at each stage

**Pipeline Coverage Starting Assumptions** (illustrative; set your own from your win rate):
| Growth Target | Required Coverage |
|---------------|-------------------|
| Aggressive (50%+ growth) | 4-5x |
| Standard (20-50% growth) | 3-4x |
| Conservative (<20% growth) | 2.5-3x |

### 5. Sales & Marketing Alignment

- [ ] Shared ICP document exists
- [ ] ICP reviewed quarterly (minimum)
- [ ] Common definitions for stages/terms
- [ ] Regular pipeline review meetings
- [ ] Feedback loop on lead quality

**ICP Document Should Include:**
- Company size (employees and/or revenue)
- Industry/vertical
- Geography
- Technology indicators
- Buying signals/triggers
- Disqualification criteria

### 6. Speed to Lead by Segment

- [ ] Different SLAs for different segments
- [ ] Enterprise leads: <5 minute response
- [ ] Mid-market leads: <15 minute response
- [ ] SMB leads: <1 hour response
- [ ] Automated alerts for SLA breaches

### 7. Renewal & Expansion

- [ ] Customer health score exists
- [ ] Health data surfaced before renewal
- [ ] Usage data integrated with CRM
- [ ] Support tickets visible to CSMs
- [ ] Expansion playbooks documented

**Customer Health Score Components:**
- Product usage (logins, feature adoption)
- Support ticket trends
- NPS/CSAT scores
- Contract utilization
- Champion engagement
- Payment history

### 8. Data Quality

- [ ] Contact data enrichment in place
- [ ] Duplicate detection running
- [ ] Required fields enforced
- [ ] Data decay audit (quarterly)
- [ ] Integration sync verification

---

## Starting Assumptions by Industry

Illustrative inputs for the calculator below, not measured benchmarks. Replace every value with your own CRM numbers before you size a leak.

### SaaS
| Metric | Starting assumption |
|--------|-----------|
| Lead Response Time | <5 min |
| MQL to SQL Conversion | 15% |
| Sales Cycle | 45 days |
| Win Rate | 25% |
| Average Deal Size | 15,000 USD |

### FinTech
| Metric | Starting assumption |
|--------|-----------|
| Lead Response Time | <5 min |
| MQL to SQL Conversion | 12% |
| Sales Cycle | 75 days |
| Win Rate | 20% |
| Average Deal Size | 35,000 USD |

### HealthTech
| Metric | Starting assumption |
|--------|-----------|
| Lead Response Time | <10 min |
| MQL to SQL Conversion | 10% |
| Sales Cycle | 100 days |
| Win Rate | 18% |
| Average Deal Size | 50,000 USD |

### DevTools
| Metric | Starting assumption |
|--------|-----------|
| Lead Response Time | <5 min |
| MQL to SQL Conversion | 15% |
| Sales Cycle | 50 days |
| Win Rate | 24% |
| Average Deal Size | 25,000 USD |

---

## Revenue Leak Calculator

### Lead Response Leak

(Current response rate - Benchmark response rate) × Monthly leads × Conversion rate × Deal size × 12

### Routing Leak

Misrouted leads per month × Conversion rate delta × Deal size × 12

### Handoff Leak

(Benchmark MQL to SQL - Actual MQL to SQL) × Monthly MQLs × Opportunity value × 12

### Churn Leak

(Benchmark retention - Actual retention) × ARR

---

## Tools Referenced

**CRM:** Salesforce, HubSpot, Attio
**Routing:** LeanData, Chili Piper, Default
**Enrichment:** Clearbit, ZoomInfo, Apollo
**Engagement:** Outreach, Salesloft, Amplemarket
**Revenue Intelligence:** Gong, Clari, Attention

---

## Automated Audit

Don't want to run this manually?

Artemis, the AI GTM Engineer, runs a GTM audit in one session inside your own Claude Code, claude.ai or Codex:

```
/plugin marketplace add tomregan-revenueleaks/artemis-gtm-plugins
/plugin install gtm-engineer@artemis-gtm
```

Free. No signup. Details: [artemisgtm.ai/engineer](https://artemisgtm.ai/engineer/)

---

## Contributing

Found a metric or benchmark we should add? Open a PR or issue.

## License

MIT. Use this however you want.

---

Built by Tom Regan | [https://artemisgtm.ai](https://artemisgtm.ai)
