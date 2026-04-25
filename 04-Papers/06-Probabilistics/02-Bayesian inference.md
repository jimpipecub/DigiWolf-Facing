## Concept
Transforms probability into a framework for updating beliefs with evidence.
## Where to begin
Conditional probability, random variables, and the law of total probability, because Bayes' rules sits upon those ideas.
## Requirement
Comfort with discrete and continuous distributions, especially [[Bernoulli]], [[Binomial]], [[Beta]], and [[Normal]] due to showing up constantly in intro Bayesian examples.

Study Path
1. Review [[03-Conditional probability|conditional probability]] and [[Bayes' theorem]]
2. Work through one or two coin-flip examples by hand.
3. Learn conjugate priors, especially Beta-Binomial and Normal-Normal
4. Move to posterior summaries: mean, creditable interval, MAP estimate.
5. Study model checking and comparison, due to the work is not just about updating but also about testing whether the model is reasonable.

Bayesian probability is often treated as a measure of uncertainty about unknown quantities, not only long-run frequency. The shift of interpretation is normally the biggest conceptual hurdle, but also makes Bayesian inference useful for decision-making and learning from limited data.

## Observation
Which poses to me a link in a way to the scientific method. Diving into that link.
## Connection
Scientific method <-> Bayesian inference

Scientific method starts with observation, hypothesis, test, and revises the hypothesis based on data. Bayesian resonance fits the pattern since it formalizes how a hypothesis changes when new evidence arrives: prior plus data produces a posterior.

A good work flow:
1. Define the question or hypothesis.
2. Write down the assumptions explicitly.
3. Choose a prior that matches starting uncertainty.
4. Compute the likelihood from observed data.
5. Update to the posterior and interpret the result.

Which pushes it less like abstract math and more like structured reasoning under uncertainty.

## Observation
It pushes the concept of what I call baselining. The exploration of that.

## Connection
Reference behavior the model expects before or after fitting. Prior predictive checks test whether the prior generates plausible data, and posterior predictive checks test if the fitted model reproduces key features of the observed data which signals the need for refinement rather than just a new posterior estimate.

## Note
"Baseline" is not always the standard word in this, but the concept is present in prior predictive checking, posterior predictive checking, and model diagnostics.

## Observation
Which hints upon the link between Drift and baseline.

## Connection
Drift means the data-generating process is no longer well represented by the same prior-plus-likelihood setup. When it occurs, posterior predictive simulations stop resembling real data in the features, which is a standard sign that the model needs revision.

A "failed predictive check" normally means the replicated data from the model systematically differs from the observed data, not just by random noise. Common mismatches include shifts in mean, variance, tail behavior, skew, multimodality, or autocorrelation structure.

## Note
When drift occurs, observed data falls outside the posterior predictive baseline, so the model fails the predictive check and should be revised or respecified. Encouraging workflow and baselining in coherence.

## Observation.
Picked to review [[03-Conditional probability|Conditional probability]]

## Core framing