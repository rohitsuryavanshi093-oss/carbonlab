CarbonLab — Evidence Matrix v1.0

Purpose

This document defines the quantitative and qualitative evidence CarbonLab will attempt to collect for its initial six CDR pathways.

The matrix is a research specification, not a dataset. Values will only be added after their sources, definitions, units, and system boundaries have been checked.

---

1. Core Pathways

CarbonLab v0.1 initially considers:

1. Afforestation / Reforestation (A/R)
2. Soil Carbon Sequestration (SCS)
3. Biochar
4. Bioenergy with Carbon Capture and Storage (BECCS)
5. Direct Air Carbon Capture and Storage (DACCS)
6. Enhanced Weathering (EW)

---

2. Evidence Categories

Each pathway will be investigated across the following categories.

A. Carbon removal

Variable| Meaning| Preferred unit
Gross removal| CO₂ captured from atmosphere before additional emissions| tCO₂
Net removal| Atmospheric CO₂ removal after relevant lifecycle emissions| tCO₂
Annual removal rate| Removal achieved per unit time| tCO₂/year
Removal efficiency| Fraction of potential carbon ultimately stored| %

---

B. Cost

Variable| Meaning| Preferred unit
Removal cost| Cost associated with removing one tonne of CO₂| USD/tCO₂
Capital cost| Upfront infrastructure cost where available| USD
Operating cost| Ongoing operating cost where available| USD/tCO₂ or USD/year
Cost year| Year associated with monetary value| year
Currency basis| Currency and conversion assumptions| documented

Cost values must never be compared without checking their system boundary and monetary year.

---

C. Energy

Variable| Meaning| Preferred unit
Electricity requirement| Electricity needed per unit removal| MWh/tCO₂
Heat requirement| Thermal energy requirement| MWhₜₕ/tCO₂
Fuel requirement| Fuel consumption where relevant| documented unit
Total energy| Combined energy requirement where defensible| MWh/tCO₂

Energy values must specify whether they represent primary energy, final energy, electricity, heat, or another definition.

---

D. Land

Variable| Meaning| Preferred unit
Land requirement| Land associated with deployment| ha/tCO₂ or ha/GtCO₂
Land-use type| Type of land required| categorical
Land competition| Potential competition with food, biodiversity, etc.| qualitative/quantitative
Geographic dependency| Dependence on location| qualitative

---

E. Water

Variable| Meaning| Preferred unit
Water requirement| Water consumption or withdrawal where available| m³/tCO₂
Water source| Freshwater, seawater, etc.| categorical
Geographic dependency| Sensitivity to local water availability| qualitative

Water consumption and water withdrawal must not be treated as identical variables.

---

F. Permanence and storage

Variable| Meaning| Preferred unit
Storage medium| Where removed carbon is stored| categorical
Storage duration| Expected storage timescale| years
Reversal risk| Risk of stored carbon returning to atmosphere| qualitative/quantitative
Monitoring requirement| Monitoring needs| qualitative

CarbonLab should preserve storage-duration differences rather than treating all tonnes of CDR as equivalent.

---

G. Deployment and maturity

Variable| Meaning
Current deployment| Present deployment level
Technology maturity| Maturity/readiness assessment
Commercial status| Research/pilot/demonstration/commercial/etc.
Scale-up rate| Plausible deployment growth
Infrastructure requirements| Major infrastructure needs

---

H. Environmental and social dimensions

Potential variables:

- Biodiversity impacts
- Ecosystem effects
- Food-system interactions
- Mineral/resource extraction
- Local environmental effects
- Additional emissions
- Social considerations
- Governance requirements

These variables may initially remain qualitative if comparable quantitative data do not exist.

---

3. Evidence Record Structure

Every quantitative observation should ultimately have a record containing:

Pathway
Variable
Value
Unit
Source
Publication year
Data year
Geography
System boundary
Methodology
Source location
Transformation
Uncertainty
Notes
Evidence quality

---

4. Source Hierarchy

CarbonLab should prioritize sources approximately in this order:

Tier 1 — Major scientific assessments

Examples:

- IPCC
- State of Carbon Dioxide Removal
- National Academies
- Other major scientific assessment bodies

Tier 2 — Peer-reviewed primary research

Especially:

- Systematic reviews
- Meta-analyses
- Techno-economic assessments
- Lifecycle assessments
- Experimental studies
- Large modeling studies

Tier 3 — Government and intergovernmental datasets

Where appropriate.

Tier 4 — Institutional technical reports

Only when methodology and provenance are sufficiently transparent.

Tier 5 — Secondary summaries

Useful for discovery, but not preferred as the final source for important quantitative inputs.

---

5. Evidence Quality

Each important evidence record should receive an evidence-quality classification.

High

Strong methodology, clear system boundary, credible source, relevant to the variable and pathway.

Medium

Useful evidence but with notable limitations, assumptions, or uncertainty.

Low

Limited evidence, substantial uncertainty, or weak comparability.

Low-quality evidence may be retained for transparency but should not automatically drive major conclusions.

---

6. Comparability Rules

Two numerical values should not automatically be combined merely because they have the same unit.

Before combining values, check:

1. Same or compatible definition
2. Same system boundary
3. Compatible geographic scope
4. Compatible time period
5. Compatible currency basis
6. Compatible lifecycle accounting
7. Compatible storage definition
8. Compatible functional unit

If compatibility cannot be established, the records remain separate.

---

7. Uncertainty Rules

CarbonLab should distinguish between:

Reported uncertainty

Uncertainty explicitly provided by the source.

Derived uncertainty

Uncertainty calculated from reported data using a documented method.

Scenario range

Different values representing alternative assumptions rather than statistical uncertainty.

Expert/qualitative uncertainty

Important uncertainty that cannot reasonably be represented numerically.

These categories must not be mixed without explanation.

---

8. Missing Data

A missing value must remain missing.

CarbonLab must not silently replace missing data with:

- zero
- average values
- invented estimates
- values copied from unrelated pathways

If imputation is eventually necessary for a specific research experiment, the method must be documented separately and sensitivity-tested.

---

9. Initial Evidence Collection Priorities

The first quantitative evidence collection should prioritize:

1. Current CDR deployment/removal
2. Cost
3. Removal potential
4. Energy requirements
5. Land requirements
6. Water requirements
7. Storage duration/permanence
8. Deployment/maturity
9. Major environmental/resource constraints
10. Uncertainty

Not every variable will be available for every pathway.

---

10. Initial Data Sources

The 2026 State of Carbon Dioxide Removal data portal should be investigated first because it provides open-access datasets associated with the third edition of the report.

Relevant sections include:

- Research and development
- Demonstration and upscaling
- Current levels of CDR
- Paris-consistent CDR scenarios
- The CDR gap

The portal's datasets should be downloaded and inspected before deciding which variables can directly populate CarbonLab.

Additional peer-reviewed and assessment sources will be added where the State of CDR data do not provide sufficient pathway-level information.

---

11. First Evidence Audit

Before building the database, CarbonLab should answer:

For each pathway:

What data exist?
        ↓
What variables exist?
        ↓
What are their units?
        ↓
What are their definitions?
        ↓
What are their system boundaries?
        ↓
How uncertain are they?
        ↓
Are they actually comparable?

Only after this audit should the final database schema be frozen.

---

12. Research Principle

CarbonLab does not begin with the assumption that one CDR pathway is "best."

It begins with:

«What does the evidence actually allow us to conclude?»

The purpose of the evidence matrix is therefore to preserve the differences, uncertainty, and limitations in the underlying literature rather than forcing every pathway into an artificial single score.
