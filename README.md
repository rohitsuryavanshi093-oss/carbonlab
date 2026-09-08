CarbonLab

An open, reproducible computational laboratory for investigating carbon-dioxide-removal pathways under cost, resource, energy, and uncertainty constraints.

Overview

CarbonLab is a research-oriented computational platform for studying and comparing carbon-dioxide-removal (CDR) pathways using transparent data, quantitative models, uncertainty analysis, and scenario-based optimization.

The goal is not to declare a single "best" carbon-removal technology.

Instead, CarbonLab is designed to provide a reproducible framework for asking:

- What assumptions drive the performance of different CDR pathways?
- How do cost, energy, resource requirements, permanence, and other constraints affect comparisons?
- How sensitive are conclusions to uncertain parameters?
- Under different scenarios, which combinations of pathways remain feasible?
- How robust are technology comparisons when assumptions change?

Project Motivation

Carbon removal is likely to involve multiple approaches with different characteristics, including differences in technological maturity, cost, energy requirements, resource requirements, permanence, environmental impacts, and deployment constraints.

CarbonLab explores these differences computationally.

The project grew from an earlier student interest in carbon removal and participation in brainstorming related to the Carbon Removal XPRIZE. That earlier activity was exploratory and was not an official competition entry.

CarbonLab is an independent computational research project building on that interest.

Core Architecture

CarbonLab is organized around several connected research components:

                         CARBONLAB
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
   EVIDENCE ENGINE     MODELING ENGINE     RESEARCH ENGINE
        │                   │                   │
        │              Cost models        Experiments
        │              Energy models      Statistics
        │              Uncertainty        Sensitivity
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

1. Evidence Engine

A structured, provenance-aware database of information about CDR pathways.

The evidence layer is intended to record:

- source
- publication
- parameter
- units
- technology/pathway
- geographical context
- time period
- assumptions
- uncertainty
- methodological notes
- provenance

2. Modeling Engine

Quantitative models for evaluating pathways under defined assumptions.

Potential model categories include:

- cost
- energy
- material/resource requirements
- deployment constraints
- permanence
- environmental/resource indicators

3. Sensitivity & Uncertainty Engine

The system will investigate how uncertainty in input parameters affects model outputs.

Methods may include:

- one-at-a-time sensitivity analysis
- parameter sweeps
- probabilistic analysis
- Monte Carlo simulation
- uncertainty propagation
- robustness analysis

The exact methods will be selected based on the available evidence and research question.

4. Optimization Lab

A constrained scenario and portfolio optimization component.

Potential questions include:

«Given a set of constraints, what combinations of CDR pathways satisfy a specified removal objective?»

Possible constraints may include:

- cost
- energy
- resource availability
- deployment limits
- permanence
- uncertainty
- pathway-specific bounds

Optimization objectives and constraints will be explicitly documented rather than hidden inside the software.

5. ML Research Module

Machine learning will only be introduced where a defensible dataset and research question exist.

The project will not add machine learning simply to make the application appear more advanced.

Any ML component will include:

- clearly defined prediction target
- documented dataset
- train/test methodology
- baseline model
- evaluation metrics
- limitations
- reproducibility information

6. Research Interface

A unified interface will allow users to explore:

- evidence
- model assumptions
- pathway comparisons
- scenarios
- uncertainty
- optimization results
- research outputs

An optional AI research assistant may later provide an evidence-grounded interface to CarbonLab's underlying data and sources.

Research Principles

CarbonLab follows several principles:

Reproducibility

Important results should be reproducible from documented inputs, assumptions, code, and computational procedures.

Provenance

Important quantitative inputs should have traceable sources.

Transparency

Assumptions should be visible rather than hidden.

Uncertainty

Where scientific or economic parameters are uncertain, that uncertainty should be represented rather than ignored.

No fabricated evidence

CarbonLab will not fabricate:

- data
- citations
- experimental results
- model outputs
- research findings
- competition participation
- institutional affiliations

Research before conclusions

The project will not assume a preferred CDR technology or predetermined result.

Conclusions should emerge from the documented evidence, assumptions, models, and experiments.

Current Status

Status: Early development

The repository is currently being established.

Planned development stages include:

- [ ] Research reconnaissance
- [ ] Evidence/data architecture
- [ ] Initial CDR dataset
- [ ] Evidence explorer
- [ ] Cost and resource modeling
- [ ] Sensitivity analysis
- [ ] Uncertainty engine
- [ ] Scenario analysis
- [ ] Optimization laboratory
- [ ] ML module, if justified
- [ ] Integrated research interface
- [ ] Automated testing
- [ ] Reproducibility workflow
- [ ] Research documentation
- [ ] Research paper/report

Technology Direction

The project is expected to use a combination of:

- Python for scientific computing, analysis, modeling, optimization, and research experiments
- PostgreSQL/Supabase for structured data where appropriate
- React/TypeScript for the interactive application layer
- Git/GitHub for version control and reproducibility
- Appropriate scientific Python libraries for statistics, optimization, visualization, and machine learning where justified

The exact technology choices may evolve during development and will be documented in the repository.

Repository Structure

The project is expected to develop toward a structure similar to:

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
│   ├── research/
│   └── interview_knowledge_base.md
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── metadata/
│
├── notebooks/
│
├── src/
│   ├── evidence/
│   ├── modeling/
│   ├── sensitivity/
│   ├── uncertainty/
│   ├── optimization/
│   └── ml/
│
├── tests/
│
└── app/

This structure is provisional and will evolve as the research architecture becomes clearer.

Research Outputs

Potential outputs include:

1. An open computational framework
2. A provenance-aware CDR evidence dataset
3. Reproducible computational experiments
4. Sensitivity and uncertainty analyses
5. Scenario and optimization studies
6. Where justified, a machine-learning experiment
7. A technical research report or paper

The final research question and conclusions will be determined by the evidence and results produced during development.

Development Philosophy

CarbonLab prioritizes:

Scientific rigor > flashy features

Reproducibility > complexity

Transparent assumptions > hidden assumptions

Evidence > predetermined conclusions

Useful computation > unnecessary AI

AI-Assisted Development

AI tools may be used during software development, research organization, debugging, documentation, and implementation.

AI assistance will not be represented as independent human authorship.

The repository will maintain an AI disclosure describing the role of AI tools in development.

License

See "LICENSE" for the terms governing use of the software.

---

CarbonLab is an evolving research project.

The repository will document its development, assumptions, methods, experiments, limitations, and results as the project progresses.
