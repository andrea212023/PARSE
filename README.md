# PARSE
Protocol for responsible AI and data governance in humanitarian health settings

# PARSE

**Protocol for Privacy, Algorithmic fairness, Responsible AI, and Structural equity in Evidence-based healthcare in conflict settings**

PARSE is a protocol and training framework for medical professionals, coordinators, and data managers working in conflict-affected areas. It provides practical guidance on how to use LLMs and data analysis tools without endangering patient privacy, and introduces a bias framework specific to war-zone health data.

## The problem

93% of humanitarian professionals use AI tools for work. 9% of organizations have governance for it. In 2022, the ICRC was hacked and 515,000 vulnerable people's data was exposed. No existing framework addresses LLM governance, conflict-specific data bias, and structural equity together.

## What PARSE includes

- **Protocol document** with four data sensitivity tiers, three LLM architectures (A: LLM builds tools, B: de-identified data, C: local model), a de-identification standard, and incident response procedures
- **Five conflict-specific bias mechanisms** absent from mainstream algorithmic fairness literature: survivorship/access bias, conflict-topology bias, temporal non-stationarity, MNAR as default, and the protected-attribute paradox
- **Six-stage bias chain** tracing distortion from pre-existing inequity through collection, digitization, transmission, analysis, and decision
- **De-identification checker** (standalone HTML, works offline) that flags sensitivity risks in text before it is sent to an external LLM
- **NLP topic modelling notebook** analyzing 400+ MSF public reports from 12 conflict zones to detect reporting bias across medical themes
- **Interactive protocol website** with all resources, fairness checklist, and decision flowchart
- **Newsletter template** for ongoing dissemination
- **7 MOOC-style video scenarios** for training

## Repository structure
PARSE/
├── protocol/ # Protocol document
├── tools/
│ ├── deid-checker/ # De-identification checker (HTML)
│ └── nlp/ # Topic modelling notebook
├── website/ # Interactive protocol site
├── newsletter/ # Newsletter template
├── diagrams/ # Decision flowchart, project workflow
└── proposal/ # Project proposal document

## Keywords

Privacy, Algorithmic fairness, Responsible AI, Structural equity, Evidence-based

## Team

A.-M. Kis, M. De Jesus, M. Doudoux-Arnaud, M. Nuruzzaman

Universite Paris Cite · AIRE Programme · CorrelAid · 2026

## License

CC BY-SA 4.0
