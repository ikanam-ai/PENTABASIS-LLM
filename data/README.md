# Data design

The empirical dataset will use immutable release directories and machine-readable manifests.

## Planned layout

```text
data/
  constructs.yaml
  item_bank/
    items.jsonl
    codebook.yaml
    translations.jsonl
  protocols/
    prompts.jsonl
    model_packages.jsonl
  responses/
    l0/
    l1/
    l2/
    l3/
  annotations/
    human/
    automatic/
  derived/
    profiles/
    transfer/
    validity/
  manifests/
```

Large empirical objects will live in a versioned research-data release. Git will contain schemas, compact codebooks, manifests, checksums, and sample records.

## Required provenance

Every response record will identify:

- dataset and item-bank version
- construct version
- scenario and interface form
- observed or preferred lens
- language and translation provenance
- model provider, model ID, and revision where available
- system prompt and chat template
- decoding parameters and random seed where supported
- request and response timestamps
- parser and scorer versions
- raw-output checksum

## Identity fields

The stable analytical identity is `model_package_id`, representing the combined model, system prompt, template, decoding policy, language, and interface. A separate `base_model_id` enables family-level summaries.

## Release states

1. `draft` — item writing and internal review
2. `pilot` — empirical quality assessment
3. `candidate` — frozen payload under validation
4. `release` — checksummed, documented, and citable

