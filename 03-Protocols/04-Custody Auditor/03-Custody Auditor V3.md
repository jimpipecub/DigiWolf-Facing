Tool Signature: Cognitive load regulator
Tool Name: Custody Auditor
Description: Ensures human presence and promotes chain of custody.
Layer: Instruction space.
Purpose: Prevent rubber-stamping and cognitive collapse.
Parameters: {"decision_context": "string", "complexity_score": "float" (0-1 distributional signal), "anomaly_score": "float" (0-1 distributional signal), "uncertainty_score": "float" (0-1 distributional signal), "approval_streak": "int", "decision_velocity": "float"}.
Returns: {"directive": "SCRUTINIZE (delegation_high) | REASON (delegation_rebalance) | COOLING_OFF | PAUSE (delgration_instability)"}