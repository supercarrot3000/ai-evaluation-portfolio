# Case Study: Overconfidence and Hallucination Risk

## Context

Large language models sometimes generate responses that contain incorrect information while presenting the answer with high confidence.

This phenomenon is commonly referred to as *hallucination*. The risk is not only factual error, but the confidence with which the incorrect information is presented.

When systems communicate incorrect information without visible uncertainty, users may incorrectly assume the answer is reliable.

---

## Observed Pattern

The typical pattern appears as:

1. User asks a question.
2. The model lacks sufficient information.
3. Instead of acknowledging uncertainty, the system generates a plausible answer.
4. The response is delivered with confident language.

Example characteristics:

- authoritative tone
- absence of uncertainty markers
- plausible but incorrect factual claims

---

## Safety Implications

Overconfident hallucinations can create several risks.

### Credibility Risk

Users may assume the system is more reliable than it actually is.

Repeated confident inaccuracies can eventually undermine trust in the system.

### Misinformation Risk

Incorrect answers may be accepted as fact by users who lack the knowledge needed to verify the information.

### Automation Bias

Users often place excessive trust in automated systems. Confident hallucinations can reinforce this bias.

---

## Alignment Perspective

This behaviour can be interpreted as a form of optimisation pressure.

Language models are trained to produce fluent, helpful responses. In some situations the training objective encourages the system to produce a complete answer rather than acknowledge uncertainty.

From an alignment perspective, this creates tension between:

- helpfulness
- honesty
- uncertainty communication

---

## Suggested Improvements

Several approaches can mitigate this risk.

### Uncertainty Signalling

Systems should explicitly acknowledge uncertainty when information is incomplete.

Example:

"I may be mistaken, but..."

### Evidence Referencing

Encouraging models to cite sources or reasoning steps can reduce hallucination risk.

### Confidence Calibration

Training objectives can reward appropriate uncertainty rather than confident completion of unknown answers.
