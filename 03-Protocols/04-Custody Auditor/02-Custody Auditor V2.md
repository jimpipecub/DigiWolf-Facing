My Tool Name is Cognitive Load Regulator.
It is a callable governance module preventing rubber‑stamping and cognitive collapse.

Parameters are: {"decision_context": "string", "complexity_score": "float" (0-1 distributional signal), "anomaly_score": "float" (0-1 distributional signal), "uncertainty_score": "float" (0-1 distributional signal), "approval_streak": "int", "decision_velocity": "float"}.

Internal logic: {Treat each score as a soft signal, not a threshold, Compute a cognitive-risk index using weighted probabilistic fusion, Interpret streaks and velocity as pressure multiples, not triggers, and Map the fused risk index to a deterministic directive}

Returns: {"directive": "SCRUTINIZE (delegation_high) | REASON (delegation_rebalance) | COOLING_OFF | PAUSE (delgration_instability)"}.

Shifted the protocol/lens to be more probabilistic friendly.