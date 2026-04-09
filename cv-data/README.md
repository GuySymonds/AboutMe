# CV Data — Guy Symonds

This folder contains the source data for Guy Symonds' CV, broken into individual components. AI tools can draw on these files to generate tailored CVs for specific roles.

## Structure

```
cv-data/
├── profile/
│   ├── contact.md                  Personal contact details
│   └── personal-statement.md      Personal statement and summary variants
├── skills/
│   ├── leadership-and-delivery.md  Team leadership, delivery governance, coaching
│   ├── technical-strategy.md       Architecture, cloud strategy, security
│   ├── engineering-practices.md    Agile, quality, standards, cross-team working
│   ├── programming.md              Languages, frameworks, and software patterns
│   ├── cloud-and-infrastructure.md Azure, IaC, databases, networking
│   ├── devops.md                   CI/CD, pipelines, containers, observability
│   └── ai-and-ml.md                LLM, RAG, ML integrations, AI governance
├── experience/
│   ├── 2024-present--newday--lead-engineer.md
│   ├── 2021-2024--elekta--engineering-manager.md
│   ├── 2020-2021--southern-water--digital-lead.md
│   ├── 2019-2020--honeywell--principal-engineer.md
│   ├── 2016-2019--adetiq--head-of-it.md
│   ├── 2014-2016--portsmouth-nhs--database-manager.md
│   ├── 2013-2014--family-investments--technical-architect.md
│   ├── 2004-2012--bond-international--infrastructure-manager.md
│   └── 1997-2004--early-career.md
└── education/
    ├── industry-qualifications.md
    ├── it-certifications.md
    └── academic.md
```

## How to Use

Each file contains a focused set of bullet-pointed facts. When generating a CV for a specific role, provide the relevant files to an AI tool along with the job description and ask it to compose a tailored CV.

For example:
- A senior engineering manager role → focus on `leadership-and-delivery.md`, `technical-strategy.md`, and recent `experience/` files.
- An AI/ML platform role → include `ai-and-ml.md`, `cloud-and-infrastructure.md`, and relevant `experience/` files.
- A hands-on lead engineer role → include `programming.md`, `devops.md`, and `engineering-practices.md`.
