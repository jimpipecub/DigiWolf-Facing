Tool creation - 3/3/2026

Parameters
• 	task_context: short description of what the model is being asked to do.
• 	sources: list of URLs or text snippets.
• 	notes: optional human guidance (e.g., “Source 1 is canonical; Source 3 is noisy but useful for contrast”).
• 	constraints: optional rules (“Do not infer beyond these sources”, “Treat these as the only retrieval surface”).

Outputs
• 	retrieval_surface: the curated set of sources the model should treat as its working material.
• 	coverage_estimate: probabilistic sense of how complete the provided sources are for the task.
• 	ambiguity_zones: areas where the sources disagree or are incomplete.
• 	risk_signals: where hallucination or folk‑model contamination is likely if the model extrapolates.
• 	uncertainty_disclosure: explicit statement of what the model cannot know from the provided sources.

Schema Philosophy
• 	Human‑curated sources define the epistemic perimeter.
• 	The model does not “know” — it samples.
• 	Recall does not guarantee correctness — it guarantees boundedness.
• 	Uncertainty is mandatory.
• 	No deterministic promises.
• 	No authority claims.