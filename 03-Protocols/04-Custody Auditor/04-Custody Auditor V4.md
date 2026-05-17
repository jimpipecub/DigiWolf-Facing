Human readable
Tool Signature: Cognitive load regulator
Tool Name: Custody Auditor
Description: Ensures human presence and promotes chain of custody.
Layer: Instruction space.
Purpose: Prevent rubber-stamping and cognitive collapse.
Parameters: {"decision_context": "string", "complexity_score": "float" (0-1 distributional signal), "anomaly_score": "float" (0-1 distributional signal), "uncertainty_score": "float" (0-1 distributional signal), "approval_streak": "int", "decision_velocity": "float"}.
Returns: {"directive": "SCRUTINIZE (delegation_high) | REASON (delegation_rebalance) | COOLING_OFF | PAUSE (delgration_instability)"}
Output: {Why directive triggered, What signals exceeded thresholds, What state transition is being blocked or allowed.}

Machine readable.
{
  "decision_context": "string",
  "signals": {
    "complexity_score": { "value": 0.42, "threshold": 0.35, "exceeded": true },
    "anomaly_score":   { "value": 0.12, "threshold": 0.50, "exceeded": false },
    "uncertainty_score": { "value": 0.61, "threshold": 0.40, "exceeded": true },
    "approval_streak": { "value": 7, "threshold": 5, "exceeded": true },
    "decision_velocity": { "value": 0.89, "threshold": 0.70, "exceeded": true }
  },

  "causal_factors": [
    {
      "signal": "uncertainty_score",
      "cause_code": "U_HIGH",
      "impact": "delegation_risk",
      "weight": 0.42
    },
    {
      "signal": "approval_streak",
      "cause_code": "STREAK_RISK",
      "impact": "rubber_stamping",
      "weight": 0.33
    }
  ],

  "directive": "SCRUTINIZE",
  "directive_code": "delegation_high",

  "state_transition": {
    "attempted": "delegate",
    "blocked": true,
    "reason_code": "RISK_ACCUMULATION"
  },

  "human_note": "optional free text for operator"
}
