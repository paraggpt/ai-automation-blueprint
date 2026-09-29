# AI ROI Calculator & Next Steps

## Simple ROI model for AI automation

For each use case, estimate:

### Inputs

- **Volume/month**: Number of items processed (leads, tickets, records, etc.)
- **Current handle time**: Avg minutes a human spends per item
- **Target time with AI**: Expected minutes after AI assistance
- **Fully loaded cost/hour**: Cost per employee hour (salary + overhead)
- **AI cost/month**: Estimated AI/API + infra cost for this use case

### Calculations

- Time saved per item = `current_handle_time - target_time_with_ai` (minutes)  
- Time saved/month (hours) = `(time_saved_per_item * volume_per_month) / 60`  
- Labor savings/month = `time_saved_per_month_hours * cost_per_hour`  
- Net monthly benefit = `labor_savings_per_month - ai_cost_per_month`  
- Annual net benefit = `net_monthly_benefit * 12`

Use this to rank use cases by **annual net benefit** and **implementation effort**.

---

## From blueprint to pilot in 30–60 days

### Week 1–2: Pick & scope

- Choose 1–2 use cases from `WORKFLOW_TEMPLATES.md`.
- Define:
  - Success metrics (e.g., response time, conversion rate, effort saved)
  - Data sources and systems involved
  - Stakeholders (sales, support, ops, IT)

### Week 2–4: Design & build MVP

- Map the workflow step‑by‑step.
- Decide:
  - Which steps are AI vs rules vs human review
- Implement a minimal version:
  - Can be a simple script + manual trigger at first
  - Or a basic integration with your CRM/helpdesk

### Week 4–8: Pilot & measure

- Run the workflow in production for a limited segment (e.g., one team/region).
- Track:
  - Time saved
  - Quality impact (conversion, CSAT, error rates)
  - User feedback
- Iterate on prompts, rules, and routing.

### After pilot

- If metrics are positive:
  - Harden the integration
  - Expand to more teams/regions
  - Add more workflows using the same pattern

---

Want help scoping and building your first AI pilot?  
Book a free 30‑min session: https://dianapps.com/contact (mention “AI Blueprint”).
