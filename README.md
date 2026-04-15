# AI Customer Support Deployment Strategy and Data Improvement Schematic

A case study presentation covering end-to-end strategy for deploying an AI-powered customer support agent in a precision medicine environment, paired with a physician health scoring framework that replaces blunt CRM labels with composite, data-driven risk tiers.

## Overview

This project addresses two connected problems in customer success operations at a diagnostics organization where 40% of CS tickets are status inquiries with answers already available in internal systems.

**Part 1: AI Agent Lifecycle Management**
Designed a retrieval-based AI agent with confidence-tiered routing (auto-reply, assisted draft, human fallback), a phased rollout from shadow mode through production, and a structured human feedback loop that turns every CS interaction into a labeled training signal. Includes a full Business Requirements Document (BRD) framework, sidecar UI spec, accuracy drift detection protocol, and KPI architecture covering deflection rate, automation accuracy, handle time, and cost-per-ticket.

**Part 2: CRM Data Improvement and Physician Health Scoring**
Built a composite Health Tier framework (Healthy, Watch, At Risk, Critical) that replaces binary Active/Inactive CRM status by joining Salesforce CRM fields with lab database records. Defined four new KPIs (Order Activity Score, Engagement Score, CS Relationship Recency, Physician Health Tier) and specified the data architecture, join keys, derived fields, and dashboard filters the BI team needs to build the monitoring layer.

**Part 3: Physician Health Dashboard**
Designed a full dashboard mockup with KPI cards, a bubble scatter plot mapping contact gaps against order trends, regional contact heatmaps, a 12-month order trend line, and a priority action table sorted by risk tier with recommended next steps per physician.

## Key Concepts

- Confidence-based routing with calibrated thresholds (shadow phase tuning)
- Retrieval-augmented generation grounded in approved internal source systems
- PII scrubbing, sentiment detection, and hard-block guardrails
- Phased rollout with defined stakeholder gates at each phase
- Human feedback loop design (accept / edit / reject) with feedback fatigue monitoring
- Accuracy drift detection and remediation when new product lines launch
- Composite health scoring replacing binary CRM classifications
- CRM-to-lab data joins for churn risk surfacing

## Tools and Frameworks Referenced

SQL, Salesforce CRM, Tableau, retrieval-based AI architecture, vector knowledge bases, sidecar UI pattern, A/B threshold calibration

## Author

**Ash Sarsour**
[GitHub](https://github.com/ashsconomist) · [LinkedIn](https://linkedin.com/in/ashsarsour)
