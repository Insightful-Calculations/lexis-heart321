# Machine-Readable Data

Structured data for programmatic consumption of QHOTS results.

## Files

| File | Description |
|------|-------------|
| `constants_derived.json` | All derived physical constants with formulas, values, uncertainties, and CODATA references |
| `predictions.json` | All falsifiable predictions with experimental targets and status |

## Schema: constants_derived.json

Each entry contains:
- `name`: Human-readable name
- `symbol`: Mathematical symbol
- `qhots_formula`: The QHOTS derivation formula
- `qhots_value`: Numerical value from QHOTS
- `experimental_value`: Best experimental measurement
- `experimental_source`: Source of experimental value
- `error_ppb`: Error in parts per billion (ppb)
- `sqrt_n_basis`: Which √n geometric base applies
- `status`: "verified", "predicted", or "tension"

## Schema: predictions.json

Each entry contains:
- `id`: Prediction number (1–54)
- `domain`: Physics domain
- `name`: Prediction name
- `symbol`: Mathematical symbol
- `qhots_formula`: Derivation formula
- `qhots_value`: Predicted value
- `experimental_target`: What experiment would test this
- `precision_required`: Required experimental precision
- `current_status`: "verified", "predicted", "consistent", or "tension"
- `relevant_experiment`: Specific experimental facility or dataset
- `error_percent`: Current error vs experiment (if measured)
- `sqrt_n_basis`: Geometric basis

All values use SI units unless otherwise specified. Error estimates are relative to experimental values where available.

## License

All data in this directory is licensed under [CC BY-SA 4.0](../LICENSE-CC-BY-SA-4.0).
