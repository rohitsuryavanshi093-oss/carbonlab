CARBONLAB — Master Specification v1.0

1. Project Identity

Project name: CarbonLab

Description:
An open, reproducible computational laboratory for investigating carbon-dioxide-removal (CDR) pathways under cost, resource, energy, permanence, deployment, and uncertainty constraints.

CarbonLab is intended to be a research-oriented computational platform rather than a generic informational website or AI chatbot.

---

2. Core Vision

CarbonLab aims to create a transparent computational environment where carbon-dioxide-removal pathways can be compared, modeled, stress-tested, and explored using traceable evidence and explicit assumptions.

The central principle is:

«Evidence → Data → Model → Uncertainty → Experiment → Optimization → Result → Interpretation»

Every important quantitative conclusion should be traceable back to the assumptions and evidence used to produce it.

---

3. Central Research Philosophy

CarbonLab must prioritize:

1. Scientific transparency
2. Reproducibility
3. Evidence provenance
4. Explicit assumptions
5. Uncertainty analysis
6. Sensitivity analysis
7. Constraint-aware optimization
8. Honest interpretation
9. Clear limitations
10. No predetermined conclusions

CarbonLab should never manipulate assumptions to produce a desired conclusion.

---

4. Primary Research Question

«How do different carbon-dioxide-removal pathways compare when cost, energy, resource requirements, permanence, deployment constraints, and parameter uncertainty are considered simultaneously?»

The exact final research question may be narrowed after evidence collection and exploratory analysis.

---

5. Secondary Research Questions

Potential secondary questions include:

- How sensitive are pathway rankings to uncertain assumptions?
- Which parameters most strongly influence pathway performance?
- How do different deployment scenarios change pathway selection?
- Can combinations of pathways outperform individual pathways under specific constraints?
- How robust are optimization results to uncertainty?
- Which trade-offs emerge between cost, energy, resource use, permanence, and scale?
- Where are existing public datasets insufficient for reliable comparison?

These questions are exploratory. CarbonLab must allow the evidence and experiments to determine the final conclusions.

---

6. Scope of CarbonLab

CarbonLab may investigate multiple CDR pathways, including but not necessarily limited to:

- Afforestation and reforestation
- Soil carbon approaches
- Biochar
- Bioenergy with carbon capture and storage
- Direct air capture
- Enhanced weathering
- Mineral-based approaches
- Ocean-based approaches
- Biomass-based approaches
- Other scientifically documented CDR pathways

Pathways should only be included in quantitative comparisons when sufficient evidence exists.

Poorly documented pathways may be represented qualitatively or excluded from quantitative analysis.

---

7. CarbonLab Architecture

CarbonLab consists of interconnected research and software layers.

                         CARBONLAB
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
   EVIDENCE ENGINE     MODELING ENGINE     RESEARCH ENGINE
        │                   │                   │
        │              Cost models        Experiments
        │              Energy models      Statistics
        │              Resource models   Sensitivity
        │              Permanence        Uncertainty
        │                   │                   │
        └───────────────────┼───────────────────┘
                            │
                     OPTIMIZATION LAB
                            │
                   Scenario exploration
                            │
                            ▼
                     ML / Prediction
                            │
                            ▼
                    RESEARCH FINDINGS
                            │
                            ▼
                      PAPER / REPORT
                            │
                            ▼
                  OPTIONAL AI ASSISTANT

The system should be modular so that individual components can be tested independently.

---

8. Evidence Engine

The Evidence Engine stores structured information about CDR pathways and their reported characteristics.

Potential fields include:

- Pathway name
- Technology/category
- Reported removal rate
- Cost
- Energy requirement
- Land requirement
- Water requirement
- Storage duration/permanence
- Technology readiness
- Deployment constraints
- Environmental considerations
- Geographic assumptions
- Source
- Publication year
- Data type
- Unit
- Confidence level
- Notes
- Citation/provenance information

The Evidence Engine must distinguish:

- measured values
- modeled values
- estimated values
- scenario assumptions
- expert assessments

---

9. Evidence Provenance

Important quantitative inputs must have traceable provenance.

For each important value, CarbonLab should attempt to record:

Value
↓
Unit
↓
Source
↓
Publication
↓
Table/Figure/Section where possible
↓
Interpretation
↓
Transformation applied

No fabricated citations or unsupported numerical values may be introduced.

If a value is derived from another value, the transformation must be documented.

---

10. Modeling Engine

The Modeling Engine converts evidence and assumptions into transparent computational models.

Potential model dimensions include:

Cost

- Cost per tonne CO₂ removed
- Capital expenditure where available
- Operating expenditure where available
- Energy-related costs
- Transport/storage assumptions where relevant

Energy

- Electricity requirements
- Heat requirements
- Fuel requirements
- Energy intensity

Resources

- Land
- Water
- Biomass
- Minerals/materials
- Infrastructure

Carbon

- Gross removal
- Net removal
- Additional emissions
- Storage duration
- Leakage/reversal assumptions

Models must clearly distinguish reported data from derived estimates.

---

11. Model Transparency

Every major model should document:

- Inputs
- Units
- Equations
- Assumptions
- Parameter ranges
- Sources
- Outputs
- Limitations

Where possible, the same calculation should be reproducible from a notebook or script without relying on the graphical interface.

---

12. Sensitivity Analysis

CarbonLab should determine which assumptions have the greatest influence on results.

Possible approaches:

- One-at-a-time sensitivity analysis
- Parameter sweeps
- Tornado-style analyses
- Correlation analysis
- Global sensitivity analysis where appropriate

Example question:

«If electricity price changes substantially, how does the relative performance of an energy-intensive CDR pathway change?»

Sensitivity analysis should be performed before making strong comparative claims.

---

13. Uncertainty Engine

CDR estimates often involve uncertain parameters.

CarbonLab should represent uncertainty explicitly rather than hiding it behind single-point estimates.

Possible distributions include:

- Uniform
- Triangular
- Normal
- Log-normal
- Empirical distributions

The distribution selected must be justified.

Potential outputs:

- Confidence/credible ranges
- Distribution of total cost
- Distribution of net removal
- Probability of satisfying constraints
- Robustness of pathway rankings

Uncertainty ranges must never be invented merely to make a result appear scientifically precise.

---

14. Scenario Engine

CarbonLab should allow users/researchers to investigate different scenarios.

Examples:

Scenario A — Cost constrained

Minimize cost while achieving a specified removal target.

Scenario B — Energy constrained

Limit available clean energy.

Scenario C — Land constrained

Limit available land.

Scenario D — Water constrained

Limit water availability.

Scenario E — Deployment constrained

Limit annual deployment growth.

Scenario F — Multi-objective

Consider cost, energy, resources, and permanence simultaneously.

Scenarios must have documented assumptions.

---

15. Optimization Engine

The Optimization Engine investigates how CDR portfolios could satisfy specified objectives and constraints.

A simplified formulation could be:

Minimize:
    Total system cost

Subject to:
    Total removal >= target
    Energy <= available energy
    Land <= available land
    Water <= available water
    Deployment <= deployment limit
    Pathway-specific constraints

The mathematical formulation should evolve as the evidence and research question develop.

Possible methods include:

- Linear programming
- Mixed-integer optimization
- Nonlinear optimization
- Multi-objective optimization

Only methods appropriate to the mathematical structure of the problem should be used.

---

16. Robust Optimization

Where uncertainty is sufficiently characterized, CarbonLab may investigate robust optimization.

The goal is not simply to find the mathematically cheapest solution under one set of assumptions.

Instead, investigate solutions that remain reasonable when uncertain parameters vary.

Potential questions:

- Does the optimal portfolio remain optimal under uncertainty?
- Which portfolios are fragile?
- Which pathways consistently contribute under different assumptions?
- What cost is associated with choosing a more robust solution?

Robust optimization must not be implemented merely as a visual feature. It must correspond to a clearly defined mathematical formulation.

---

17. ML Component

Machine learning is optional and must be justified by a real research problem and adequate data.

Possible applications include:

- Predicting pathway-level performance from structured features
- Detecting patterns across evidence
- Estimating missing values where scientifically defensible
- Clustering pathways by characteristics
- Ranking or classification experiments

CarbonLab must not add ML simply because "AI" makes the project appear more advanced.

If the dataset is too small, heterogeneous, biased, or poorly labeled, the ML component should be reduced or omitted.

---

18. Research Assistant

An optional AI research interface may eventually allow users to ask questions about CarbonLab's evidence and results.

It should be:

- Evidence-grounded
- Citation-aware
- Transparent
- Limited to available evidence
- Explicit about uncertainty
- Explicit about unsupported questions

The assistant must not become the core research contribution.

The research contribution should remain the evidence, computational methodology, experiments, and findings.

---

19. Software Architecture

Recommended software structure:

Frontend
    ↓
Application/API Layer
    ↓
Database
    ↓
Research Computation Layer
    ↓
Python Models / Experiments
    ↓
Results
    ↓
Visualization / Research Interface

The system should keep research computation separate from presentation logic.

---

20. Lovable vs Python

Lovable

Use Lovable primarily for:

- Frontend
- UI
- Navigation
- Forms
- Dashboards
- Basic backend scaffolding
- Authentication if needed
- Database integration
- Application structure

Python

Use Python for:

- Data processing
- Scientific calculations
- Statistical analysis
- Sensitivity analysis
- Uncertainty analysis
- Optimization
- ML experiments
- Research notebooks
- Reproducible experiments

The scientific computation must not depend entirely on a visual application builder.

---

21. Database Concept

A relational database may contain entities such as:

pathways
sources
evidence
parameters
scenarios
experiments
experiment_runs
model_versions
optimization_runs
results

Relationships and schema should be designed to preserve provenance and reproducibility.

Example:

Source
  ↓
Evidence Record
  ↓
Parameter
  ↓
Model
  ↓
Experiment
  ↓
Result

---

22. Reproducibility Architecture

A researcher should be able to understand:

1. What data were used
2. Where the data came from
3. What assumptions were made
4. Which model version was used
5. Which parameters were used
6. Which experiment was run
7. What output was generated

Important experiment runs should record:

- Date
- Code version/commit
- Dataset version
- Model version
- Parameters
- Scenario
- Random seed where relevant
- Output files
- Notes

---

23. Repository Structure

Target structure:

carbonlab/
│
├── README.md
├── LICENSE
├── AI_DISCLOSURE.md
├── DECISIONS.md
├── CONTRIBUTING.md
├── .gitignore
│
├── docs/
│   ├── MASTER_SPECIFICATION.md
│   ├── methodology.md
│   ├── data_dictionary.md
│   └── research_notes.md
│
├── app/
│   ├── frontend/
│   └── backend/
│
├── src/
│   ├── data/
│   ├── models/
│   ├── sensitivity/
│   ├── uncertainty/
│   ├── optimization/
│   └── ml/
│
├── research/
│   ├── notebooks/
│   ├── experiments/
│   ├── data/
│   └── figures/
│
├── tests/
│
└── configs/

The exact structure may evolve as implementation begins.

---

24. Research Notebook

The research process should maintain a structured notebook/log.

Each research experiment should record:

Research question
Hypothesis
Data
Assumptions
Method
Parameters
Experiment
Result
Interpretation
Limitations
Next question

Unexpected results must be recorded rather than discarded.

---

25. Testing Strategy

CarbonLab requires both software testing and scientific validation.

Software tests

- Unit tests
- Integration tests
- API tests
- Database tests
- Frontend tests where appropriate

Scientific tests

- Equation verification
- Unit consistency
- Boundary-condition tests
- Known-value tests
- Conservation/constraint checks
- Sensitivity sanity checks
- Reproducibility checks

A scientifically incorrect result can exist inside perfectly functioning software, so both forms of testing are required.

---

26. Data Quality Rules

Every quantitative dataset should be checked for:

- Missing values
- Duplicate records
- Unit inconsistencies
- Conflicting sources
- Outliers
- Different system boundaries
- Different definitions of "removal"
- Different geographic assumptions
- Different time periods
- Incompatible methodologies

Numbers from different sources must not automatically be treated as directly comparable.

---

27. Scientific Limitations

CarbonLab must explicitly recognize limitations including:

- Limited availability of comparable data
- Different methodological assumptions across studies
- Geographic variation
- Temporal variation
- Uncertainty in future technology costs
- Difficulty comparing fundamentally different CDR pathways
- Potential correlation between uncertain parameters
- System-boundary differences
- Data quality limitations
- Model simplifications

Limitations should be part of the research output, not hidden.

---

28. What CarbonLab Must NOT Become

CarbonLab must not become:

- A generic chatbot
- A generic AI wrapper
- A simple CRUD dashboard with no research contribution
- A collection of copied numbers without provenance
- A fake scientific simulator
- A fabricated research project
- A system with invented citations
- A system with fabricated experimental results
- A predetermined conclusion disguised as research
- A project claiming official competition participation that did not occur

The interface should support the research rather than substitute for it.

---

29. Connection to Original Carbon-Removal Interest

The project builds upon an earlier student interest in carbon removal.

The earlier activity involved brainstorming around carbon-removal technologies, studying existing approaches and their limitations, and discussing possible improvements.

It was not an official Carbon XPRIZE competition entry.

CarbonLab should honestly present this as the origin of the research interest rather than exaggerating the experience.

---

30. Research Paper Direction

A possible flagship paper direction is:

«A Reproducible Computational Framework for Evaluating Carbon-Dioxide-Removal Pathways Under Cost, Resource, and Uncertainty Constraints»

Potential alternative directions:

«Robust Portfolio Optimization of Carbon-Dioxide-Removal Pathways Under Parameter Uncertainty»

or:

«How Robust Are Carbon-Removal Technology Comparisons to Uncertain Cost and Resource Assumptions?»

The final title must be determined by the actual research performed.

The paper must not claim a novel scientific discovery before evidence supports that claim.

---

31. Paper Structure

Potential structure:

Abstract

Research question, methodology, major results, significance.

1. Introduction

- CDR context
- Motivation
- Existing challenge
- Research gap
- Research questions

2. Related Work

- Existing CDR assessment approaches
- Techno-economic studies
- Resource constraints
- Uncertainty analysis
- Optimization approaches

3. Data and Evidence

- Sources
- Dataset construction
- Provenance
- Inclusion/exclusion criteria
- Data limitations

4. Methodology

- Models
- Assumptions
- Sensitivity analysis
- Uncertainty framework
- Optimization framework

5. Experiments

- Experimental design
- Scenarios
- Parameter ranges
- Reproducibility

6. Results

- Main results
- Sensitivity
- Uncertainty
- Optimization
- Robustness

7. Discussion

- Interpretation
- Comparison with existing literature
- Implications
- Limitations

8. Conclusion

- Main findings
- What CarbonLab contributes
- Future research

Reproducibility Appendix

- Code
- Dataset versions
- Parameters
- Experiment configurations

---

32. Development Milestones

Milestone 0 — Foundation

- Repository
- Documentation
- License
- AI disclosure
- Decision log
- Specification

Milestone 1 — Evidence Foundation

- Initial pathway list
- Source records
- Evidence schema
- Provenance system
- Initial dataset

Milestone 2 — Evidence Explorer

- Search
- Filtering
- Pathway comparison
- Source display

Milestone 3 — Modeling Engine

- Cost models
- Energy models
- Resource models
- Carbon accounting

Milestone 4 — Sensitivity Analysis

- Parameter sweeps
- Sensitivity outputs
- Visualization

Milestone 5 — Uncertainty Engine

- Parameter distributions
- Monte Carlo experiments
- Result distributions

Milestone 6 — Scenario Engine

- Scenario configuration
- Constraint system
- Scenario comparison

Milestone 7 — Optimization Lab

- Objective functions
- Constraints
- Portfolio optimization
- Result interpretation

Milestone 8 — Robust Optimization

- Uncertain optimization inputs
- Robustness experiments
- Portfolio stability analysis

Milestone 9 — ML Research Module

Only if justified by the dataset and research question.

Milestone 10 — Integrated Research Interface

Connect the research engines to the application.

Milestone 11 — Testing

- Unit tests
- Scientific validation
- Reproducibility tests

Milestone 12 — Research Experiments

Run the finalized experiments.

Milestone 13 — Research Documentation

Document methods, assumptions, results, limitations, and conclusions.

Milestone 14 — Paper Draft

Produce a complete research-paper draft based on actual results.

Milestone 15 — CarbonLab v1.0

Deliver the stable research platform, documentation, experiments, and paper draft.

---

33. November 2026 Definition of Done

By November 2026, the target is a serious CarbonLab v1.0, including:

- Functional research-oriented software
- Evidence database
- Provenance system
- Transparent computational models
- Sensitivity analysis
- Uncertainty analysis
- Scenario analysis
- Optimization capability
- ML module only if scientifically justified
- Reproducible experiments
- Testing
- High-quality documentation
- Clean GitHub repository
- Research findings
- Research figures
- Paper draft
- Explicit limitations
- AI development disclosure

"Done" does not mean that every possible feature has been implemented.

It means the implemented system is coherent, reproducible, defensible, and research-ready.

---

34. AI-Assisted Development Policy

CarbonLab is being developed with significant assistance from AI tools.

AI may assist with:

- Software architecture
- Code generation
- Debugging
- Documentation
- Testing
- Research organization
- Mathematical formulation
- Computational approaches
- Literature organization
- Experiment design suggestions

AI output must not automatically be treated as fact.

All important scientific claims, sources, assumptions, equations, and results must be reviewed and validated.

CarbonLab must never fabricate:

- Research results
- Citations
- Datasets
- Experiments
- Competition participation
- Credentials
- Publications
- Human contributions

AI assistance should be transparently documented.

---

35. Quality Standard

CarbonLab should aim for the following standard:

Scientific quality

- Traceable evidence
- Explicit assumptions
- Appropriate mathematics
- Uncertainty
- Sensitivity
- Reproducibility
- Honest limitations

Software quality

- Modular architecture
- Clean code
- Testing
- Documentation
- Version control
- Maintainability

Research quality

- Clear question
- Reproducible methodology
- Experiment-driven conclusions
- No predetermined outcome
- Clear distinction between evidence and inference

Presentation quality

- Professional interface
- Clear visualizations
- Understandable explanations
- Research-first design

The project should favor rigor over visual complexity.

---

36. Immediate Next Step

After this specification is committed:

1. Conduct research reconnaissance.
2. Identify authoritative datasets and literature.
3. Define the initial pathway scope.
4. Design the evidence schema.
5. Establish provenance rules.
6. Create the initial research dataset.
7. Validate the dataset before implementing advanced models.
8. Begin CarbonLab Evidence.

No advanced optimization or ML should be implemented before the evidence foundation is sufficiently reliable.

---

37. Final Principle

CarbonLab follows this pipeline:

QUESTION
   ↓
EVIDENCE
   ↓
DATA
   ↓
MODEL
   ↓
UNCERTAINTY
   ↓
EXPERIMENT
   ↓
OPTIMIZATION
   ↓
RESULT
   ↓
INTERPRETATION
   ↓
PAPER
   ↓
SOFTWARE INTERFACE

The software exists to make the research reproducible.

The research exists to answer meaningful questions.

The conclusions must come from the evidence and experiments — not from what the project hopes to prove.

CarbonLab v1.0 is successful if another technically capable researcher can inspect the evidence, understand the assumptions, reproduce the computations, challenge the methodology, and reach their own conclusions.
