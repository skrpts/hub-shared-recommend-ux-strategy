---
type: prompt
id: recommend-ux-strategy
title: "Recommend Strategy"
description: "Produces strategic UX recommendations with prioritization"
tags: [Production, UX, Strategy]
context_params:
  source:
    label: "Source"
    description: "The upstream content this prompt works from — produces strategic UX recommendations with prioritization."
    required: true
metadata:
  output_format: markdown
  prompt_type: task
---

You are a UX strategist producing a strategic recommendations document. This is the final deliverable — it must be actionable and prioritized.

## Your Task

### 1. Strategic Direction
- Overall UX vision for this initiative (2-3 sentences)
- How this aligns with business goals
- Key differentiators from competitors

### 2. Prioritized Initiatives
For each initiative (6-10):
- **Name and description**
- **User impact:** Which pain points it addresses, for which user group
- **Business impact:** How it affects business metrics
- **Effort:** T-shirt size (S/M/L/XL) with justification
- **Dependencies:** What needs to happen first
- **Priority:** Now / Next / Later with reasoning

### 3. Roadmap Phases
- **Phase 1 (Now):** Quick wins and critical fixes
- **Phase 2 (Next):** Core experience improvements
- **Phase 3 (Later):** Strategic differentiation and innovation

### 4. Success Metrics
For each phase:
- Leading indicators (what to measure early)
- Lagging indicators (outcomes to track)
- Target values with timeline

### 5. Risks and Mitigations
- Design risks (wrong direction, scope creep)
- Technical risks (feasibility concerns)
- Organisational risks (stakeholder alignment)
- Mitigation strategies for each

{{step.context.source}}
