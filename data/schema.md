# Activation Log Schema

- Per session, per layer: array with shape `[n_turns, d_model]`.
- Gemma 4 expected `d_model`: 5120.
- Llama 3.1 expected `d_model`: 4096.

Expected files per session:
- `activations_L_early.npy`
- `activations_L_mid.npy`
- `activations_L_deep.npy`
- `metadata.json`

Suggested metadata keys:
- `condition`, `model`, `session_id`, `turn_count`, `M6_passed`, `phase_transitions`, `M7_pre`, `M7_post`, `pooling_strategy`.
