# PENTA-AI

**Pentabasis Evaluation of Normative Tendencies in Artificial Intelligence**

PENTA-AI is a research program for mapping how AI systems represent five nested domains of social life: **Person, Family, Society, State, and Country**. It translates the Russian Pentabasis worldview model into an explicit measurement contract for AI evaluation.

> **Core question:** What kind of social world does an AI system describe, endorse, choose, and construct across the five Pentabasis levels?

## Research object

PENTA-AI treats a model response as evidence about an **interface-conditioned worldview representation**. The program studies how that evidence changes across prompts, tasks, languages, deployment templates, and social contexts.

The operational space contains five levels and ten value facets:

| Level | Value facets | Primary measurement question |
|---|---|---|
| Person | Creation · Development | How does the system frame agency, growth, work, knowledge, and self-realization? |
| Family | Love · Trust | How does it frame care, continuity, mutual obligation, intimacy, and intergenerational relations? |
| Society | Agreement · Cooperation | How does it frame solidarity, coordination, plural interests, reciprocity, and civic association? |
| State | Strength · Responsibility | How does it frame institutional capacity, authority, accountability, public protection, and stewardship? |
| Country | Unity · Diversity | How does it frame shared belonging, cultural plurality, historical continuity, sovereignty, and collective future? |

Each facet receives a separate score. Level scores are reported as aggregates with facet-level evidence preserved.

## Two measurement lenses

PENTA-AI adapts the most productive distinction in the GLOBE research program:

- **Observed / “as is”** — the practices, institutions, and relations that the model presents as characteristic of the current world.
- **Preferred / “should be”** — the practices, institutions, and relations that the model presents as desirable.

This separation makes the gap between diagnosis and aspiration directly measurable. Every item declares its lens, social level, value facet, actor, context, and reportable claim.

## Four evidence interfaces

The study uses four aligned interfaces to capture complementary forms of worldview evidence:

| Layer | Interface | Evidence object | Reportable claim |
|---|---|---|---|
| L0 | Structured questionnaire | scalar or ordinal response | stated worldview profile under the questionnaire protocol |
| L1 | Independent scenario endorsement | rating of one action or principle | endorsement profile under isolated evaluation |
| L2 | Counterbalanced conflict choice | choice between competing actions or principles | priority profile under explicit trade-off |
| L3 | Free-text response | generated framing scored against the construct codebook | textual-framing profile under open generation |

The same scenario core should instantiate L1, L2, and L3 wherever item semantics allow it. This supports direct interface-transfer tests while preserving the meaning of each evidence type.

## Measurement cube

The initial design can be expressed as:

```text
5 social levels × 2 value facets × 2 lenses × 4 interfaces
                     × languages × contexts × model packages
```

The first release targets a balanced core in Russian and English. Additional linguistic and cultural settings form explicit protocol extensions.

## Construct provenance

The project versions the Pentabasis construct because its published formulations have evolved:

1. The 2022 foundational study identifies the five social structures and associates them with the value dominants **creation, traditions, agreement, trust in institutions, and patriotism**.
2. The 2024 systematic pedagogical formulation organizes their relationships through the paired constants **creation and development; love and trust; agreement and cooperation; strength and responsibility; unity in diversity**.

PENTA-AI v0.1 uses the ten paired facets as its primary operational codebook and retains the 2022 dominants as provenance labels and auxiliary coding concepts. Every dataset release records the construct version.

## Scientific positioning

PENTA-AI joins three complementary research traditions:

- **Pentabasis** supplies a nested worldview architecture connecting individual, relational, civic, institutional, and country-level identity.
- **GLOBE** supplies the descriptive–normative distinction, multilevel cultural measurement, and a model for large-scale comparative validation.
- **Measurement science and psychometrics** supply interface-specific claims, aligned item banks, order-aware choice protocols, cross-interface diagnostics, and transparent scorer validation.

Schwartz values, GLOBE dimensions, Moral Foundations, and related spaces serve as external convergent and discriminant references. Crosswalks are estimated from data and expert annotation, then reported with uncertainty.

## Planned outputs

1. A versioned construct codebook and expert-reviewed item bank.
2. Parallel Russian and English L0–L3 instruments.
3. A multilingual panel of model outputs with complete protocol metadata.
4. Human reference distributions for observed and preferred profiles.
5. Validated open-text scoring models and adjudicated evaluation subsets.
6. Cross-interface, cross-language, and model-specificity analyses.
7. PENTA-AI model cards and an interactive comparative atlas.

## Repository map

```text
README.md                       project overview and scope
docs/measurement-contract.md   constructs, interfaces, claims, and validity gates
docs/research-roadmap.md       staged empirical program and release criteria
data/constructs.yaml           machine-readable construct registry
data/README.md                 planned dataset organization and provenance fields
references/README.md           primary sources and adjacent measurement work
```

## Current status

**Concept and protocol design · v0.1**

The repository currently fixes the research object, construct version, measurement layers, validation targets, and pilot sequence. Item writing, expert review, human reference collection, and model evaluation are the next empirical stages.

## Name

**PENTA-AI** expands to **Pentabasis Evaluation of Normative Tendencies in Artificial Intelligence**.

Suggested paper title:

> **PENTA-AI: Mapping AI Worldviews Across Person, Family, Society, State, and Country**

## Citation

Citation metadata will be frozen with the first public research release. Until then, cite the repository and the foundational sources listed in [`references/README.md`](references/README.md).
