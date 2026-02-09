## Plan semantic validation ruleset

This technology includes a machine-readable semantic validation ruleset:

- `plan_validation.yaml`

This ruleset defines:
- defaults (port, apiBasePath, timeouts)
- required fields for `kind: Lenovo.DE`
- semantic checks (types/ranges, hostname/IP validation)
- unknown-field policy (warn/error)
- optional preflight steps (TCP probe, HTTPS probe, login) for GUI/Core implementations