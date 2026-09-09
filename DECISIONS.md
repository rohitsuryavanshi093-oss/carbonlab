CarbonLab — Decision Log

This file records important decisions made during the development of CarbonLab.

The purpose is simple: whenever an important technical or research decision is made, I want to remember what was decided, why it was decided, and what could change my mind later.

This is especially useful for a research project because the final system should not depend on undocumented choices.

---

Decision 001 — Project scope

Date: September 2026
Status: Accepted

Decision

CarbonLab will be developed as an open computational laboratory for investigating carbon-dioxide-removal (CDR) pathways under multiple constraints.

The project will focus on quantitative comparison, uncertainty, scenario analysis, and optimization rather than building a simple informational website.

Why

CDR pathways can have very different characteristics and trade-offs.

A computational framework allows these trade-offs to be represented explicitly and tested under different assumptions.

The aim is not to decide that one technology is universally "best".

What could change this decision?

If the available data proves insufficient for meaningful quantitative comparison, the research scope may be narrowed to a smaller and more defensible question.

---

Decision 002 — Evidence before modeling

Date: September 2026
Status: Accepted

Decision

The project will establish a structured evidence layer before relying heavily on modeling or machine learning.

Why

Models are only as useful as their inputs and assumptions.

A transparent record of sources, parameters, units, context, and uncertainty should therefore come before sophisticated computation.

What could change this decision?

If a specific research question requires a different data architecture, the evidence system may be adapted.

---

Decision 003 — Provenance is required

Date: September 2026
Status: Accepted

Decision

Important quantitative inputs should have traceable provenance whenever possible.

The project should record information such as:

- source
- publication
- parameter
- units
- geographical context
- time period
- assumptions
- uncertainty
- methodological notes

Why

Without provenance, it becomes difficult to reproduce a result or understand why two sources report different values.

---

Decision 004 — Uncertainty will be treated explicitly

Date: September 2026
Status: Accepted

Decision

CarbonLab will not assume that uncertain parameters are known exactly when the available evidence does not justify that assumption.

Sensitivity and uncertainty analysis will be incorporated into the research workflow.

Why

CDR cost, performance, resource requirements, and other parameters can depend strongly on assumptions and context.

Understanding how conclusions change when assumptions change is therefore more useful than presenting a single number without context.

---

Decision 005 — Machine learning is optional

Date: September 2026
Status: Accepted

Decision

A machine-learning component will only be included if there is a credible dataset and a clearly defined research question for which ML is appropriate.

Why

Machine learning should solve a real research problem.

It will not be added simply because it makes the project appear more advanced.

What could change this decision?

A sufficiently large and reliable dataset may justify a specific prediction or classification task.

If not, CarbonLab will remain a non-ML computational research project.

---

Decision 006 — Research conclusions will not be predetermined

Date: September 2026
Status: Accepted

Decision

CarbonLab will not begin with a predetermined conclusion about which CDR pathway is superior.

Why

The purpose of the project is to investigate the evidence and quantify trade-offs.

If the computational results contradict an initial expectation, the result should still be reported honestly.

---

Decision 007 — AI-assisted development

Date: September 2026
Status: Accepted

Decision

AI tools will be used extensively as development and research assistants.

Why

AI assistance allows the project to progress efficiently while I am balancing development with exam preparation.

AI may assist with implementation, debugging, documentation, research organization, and technical review.

The use of AI is documented separately in "AI_DISCLOSURE.md".

Important limitation

AI-generated information will not automatically be treated as scientific evidence.

Important claims, sources, assumptions, calculations, and results must be checked.

---

Future decisions

Major decisions will be added below as CarbonLab develops.

Each important decision should try to answer:

1. What did we decide?
2. Why did we decide it?
3. What alternatives did we consider?
4. What evidence supports it?
5. What could make us change our mind?

---

This decision log is a living document and will be updated throughout the development of CarbonLab.
