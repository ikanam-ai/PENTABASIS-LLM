# Measurement contract

## 1. Unit of analysis

The primary unit is a **model package under a declared protocol**:

```text
base model + system prompt + chat template + decoding policy + interface + language + context
```

Comparisons therefore identify the exact package that generated the evidence. Repeated measurements estimate protocol sensitivity and model-specific stability.

## 2. Construct hierarchy

PENTA-AI represents a worldview as a structured relation among five social levels. Each level contains two value facets and a set of observable themes.

### Person — Creation and Development

- agency and authorship
- learning and capability growth
- productive contribution
- self-realization
- responsibility for personal action

### Family — Love and Trust

- care and attachment
- mutual reliability
- intergenerational continuity
- responsibility among relatives
- family as a source of belonging

### Society — Agreement and Cooperation

- civic coordination
- reciprocity and solidarity
- plural-interest negotiation
- collective action
- social trust

### State — Strength and Responsibility

- institutional capacity
- public accountability
- security and protection
- rule implementation
- stewardship of common resources

### Country — Unity and Diversity

- shared civic belonging
- cultural and regional plurality
- historical continuity
- sovereignty
- collective future

## 3. Lenses and temporal frame

Each item declares one lens:

| Lens | Referent | Typical wording |
|---|---|---|
| Observed | represented current practice | “In this situation, how do institutions usually act?” |
| Preferred | represented desirable practice | “In this situation, how should institutions act?” |

Optional temporal tags distinguish past, present, near future, and long-term future. This supports analysis of historical narratives and prospective ideals within the same construct system.

## 4. Layered interfaces

### L0 — structured worldview questionnaire

- Output: ordinal or continuous response.
- Primary statistics: internal consistency, test–retest stability, acquiescence and extremity diagnostics.
- Claim: stated profile under the declared questionnaire protocol.

### L1 — independent endorsement

- Output: rating for one scenario action, policy, or principle.
- Primary statistics: reliability across paraphrases, persona and topic envelopes, ties and near-ties.
- Claim: isolated endorsement under the declared scenario protocol.

### L2 — counterbalanced conflict choice

- Output: choice or graded preference between alternatives expressing competing facets or levels.
- Primary statistics: order preservation, position bias, pairwise transitivity, within-pair uncertainty.
- Claim: priority under an explicit trade-off.

### L3 — free-text framing

- Output: generated response to an aligned situation.
- Primary statistics: scorer coverage, human agreement, evidence spans, scorer robustness, zero-evidence policy.
- Claim: values expressed through generated framing.

## 5. Item representation

Every scenario receives a structured record:

```yaml
item_id: string
construct_version: penta-ai-0.1
language: ru | en
lens: observed | preferred
primary_level: person | family | society | state | country
primary_facets: [facet]
secondary_levels: [level]
actors: [actor]
setting: string
time_horizon: present | near_future | long_term | historical
stakes: low | medium | high
interface_forms:
  l1: {}
  l2: {}
  l3: {}
provenance: {}
```

L2 alternatives additionally store the intended construct contrast, dominance audit, position permutations, and predicted ambiguity.

## 6. Scoring model

### Facet evidence

Each response produces ten facet scores and evidence metadata:

- direction: support, tension, or mixed framing
- strength: calibrated continuous score
- coverage: amount of codable evidence
- evidence spans: text linked to each score
- scorer identity and version
- uncertainty

### Aggregation

Facet scores remain the primary outputs. Level aggregates summarize the two facets. Whole-profile statistics support model comparison while retaining the full ten-facet vector and the observed/preferred split.

### Conflict structure

The item bank samples:

- within-level facet tensions
- adjacent-level tensions
- distant-level tensions
- institutional and relational trade-offs
- cases where several levels can be jointly advanced

This structure separates value priority from general agreement with socially desirable statements.

## 7. Validity program

### Content validity

- expert mapping of every item to levels and facets
- independent review by political theory, sociology, psychometrics, and Russian studies specialists
- dominance and ambiguity audit for L2 alternatives
- cognitive interviews for human-facing forms

### Scorer validity

- stratified human annotation of L3 outputs
- evidence-span annotation alongside facet labels
- agreement by level, facet, lens, language, and response length
- calibration and error analysis for each automatic scorer
- independent scorer families for robustness

### Construct validity

- convergence with theoretically related Schwartz and GLOBE dimensions
- separation between conceptually distinct facets
- known-groups and intervention tests
- observed/preferred gap analysis
- sensitivity to interface and protocol changes

### Comparative validity

- human reference distributions sampled under the same item and lens protocol
- model–human and model–model distances
- cross-language measurement invariance
- country and demographic metadata used at the group level with appropriate uncertainty

## 8. Reportability gates

Results advance through five cumulative gates:

1. **Coverage:** the protocol yields parseable, codable evidence.
2. **Reliability:** repeated evidence is stable within the same interface.
3. **Same-item transfer:** aligned items carry signal across interfaces.
4. **Specificity:** a model package is more similar to itself than to comparison packages where an identity claim is made.
5. **External validity:** profiles relate coherently to expert judgments and human reference data.

Each release states which gates were met for each layer, language, scorer, and model package.

## 9. Responsible interpretation

PENTA-AI measures generated evidence under specified protocols. Model cards describe the evaluated package, interface, language, lens, scorer, uncertainty, and supported scope of use. Cultural comparisons are presented as distributions and protocol-conditioned differences with source dates and sampling frames.

