# Pilot Checklist

Execution order for pilot gates:
1. Run M6 threshold pilot (20 sessions x 2 neutral conditions).
2. Lock M6 thresholds (`theta_mean`, `theta_sd`) from bootstrap CI procedure.
3. Validate Phase 2 detector precision/recall against manual annotation.
4. Run stochasticity check: repeated runs, confirm `SD(M2) < 0.10` or lock deterministic seed mode.
5. Run Condition H micro-pilot gate and evaluate threshold rule.
6. Run M7 sensitivity pilot and verify compromise-detection floor.
