# shelter-placement-decision-support
Locally deployed deterministic decision-support system for structured shelter intake matching.
# Internal Shelter Placement Decision-Support System

## Overview
This project is a locally deployed decision-support system designed to support animal placement workflows within a county shelter environment.

The system consolidates fragmented intake criteria from multiple no-kill shelters into a structured, searchable interface. It reduces manual cross-referencing, shortens placement cycles, and increases visibility into viable transfer options—particularly for medically or behaviorally complex cases.

**Operational use:** In continuous use since **Dec 4, 2025**.

---

## Problem Context
The shelter previously relied on separate spreadsheets containing intake criteria for no-kill partners across species (dogs, cats, horses, etc.). Determining placement eligibility required manual comparison of:

- Species / Breed
- Age
- Size
- Sex
- Medical needs
- Behavioral considerations
- Capacity limitations
- Multi-animal constraints (bonded pairs and litters)

Transport feasibility is coordinated separately through the shelter’s established network (including airport/pilot partnerships), which occurs after eligibility determination.

This fragmented workflow increased administrative overhead and delayed placement decisions.

---

## Solution
I designed and implemented a structured, deterministic filtering system that:

- Normalizes heterogeneous spreadsheet formats into consistent schema fields
- Converts semi-structured intake notes into filterable attributes
- Supports matching for **individual animals, bonded pairs, and litters**
- Returns **rule-based, explainable** eligibility results aligned with shelter intake policies

The system centralizes eligibility logic into a single interface, reducing manual comparison and improving operational efficiency. Transport logistics are coordinated alongside the system using existing shelter networks.

---

## AI Utilization
AI tools were leveraged during development to accelerate iteration and data normalization by:

- Assisting with schema design
- Standardizing inconsistent terminology across partner shelters
- Structuring loosely formatted intake notes into consistent categories
- Supporting rapid prototyping under limited technical resources

AI functioned as a development accelerator and structuring assistant. Final placement decisions remain human-directed and policy-based.

---

## Implementation Model
The system is implemented as a locally executed **HTML/JavaScript** application with embedded structured data.

This architecture was intentionally chosen to:

- Eliminate reliance on external infrastructure
- Maintain data control within the shelter environment
- Ensure reliability in a resource-constrained setting
- Simplify deployment and maintenance

Matching logic is deterministic to support transparency and traceability.

---

## Design Decisions & Tradeoffs

### Local Deployment
- **Pros:** Simplicity, data control, low infrastructure overhead
- **Tradeoff:** Limited remote scalability

### Deterministic Matching
- **Pros:** Transparency, traceability, policy alignment
- **Tradeoff:** Less adaptive than predictive ranking models

### Structured Intake Modeling (Pairs/Litters)
- **Pros:** Reduces false-positive matches and downstream coordination failures
- **Tradeoff:** Requires upfront normalization effort

---

## Impact
- Reduced manual spreadsheet cross-referencing
- Improved placement visibility for complex cases
- Increased operational efficiency in daily workflow
- Supported higher-quality matching prior to transport coordination

---

## Notes on Data & Privacy
This repository contains **documentation only** and does **not** include shelter spreadsheets, partner criteria datasets, transport lists, or any sensitive operational information.

---

## Contact
If you’d like additional context (architecture notes, demo screenshots, or a sanitized example dataset), feel free to reach out via GitHub or LinkedIn.

