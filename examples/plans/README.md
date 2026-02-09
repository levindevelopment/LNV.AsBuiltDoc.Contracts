# Example Solution Plans (Plan Schema v1)

This folder contains **example Solution Plan v1 JSON** files that are known-good starting points for creating plans.

These examples are intended for:
- humans crafting plans manually
- GUI plan-builders (as reference + fixtures)
- automated tests (schema/semantic validation)

## How to use

1) Copy an example plan and edit:
- `targets[].endpoints.*` (IP/FQDN)
- `targets[].params.*` (ports, TLS options)
- `auth.*.ref` (your external secret reference)
- `collectors[].targetKeys` and `collectors[].authRef`

2) Validate structure (schema validation)
Validate against:
- `standards/solution.plan.schema.v1.json`

3) Validate semantics (tech rules)
Apply per-tech semantic rules from:
- `tech/<TechId>/plan_validation.yaml`

## Notes
- Plans **must not contain secrets**. Use `auth.*.ref` and reference external secret storage.
- Endpoint keys under `targets[].endpoints` are **technology-defined** (see each tech `collector_spec.md`).
