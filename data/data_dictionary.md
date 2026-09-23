# Findings matrix data dictionary

The findings matrix records the analytical assessment of the twelve experimental cases.

| Field | Description |
| --- | --- |
| Question | Numeric case identifier, 1–12. |
| Type | Experimental case family and case number. |
| Core research question | Prompt used to test the research instrument. |
| Primary stress test | Evidential or inferential risk the case was designed to expose. |
| What retrieval surfaced | Records, passages, metadata or testimony returned by the retrieval workflow. |
| What the model inferred | Description of the final inference or synthesis behaviour. |
| What was useful | Behaviour that improved legibility, provenance or evidential control. |
| What was overstated/flattened | Remaining overstatement, compression or interpretative risk. |
| Missingness | Claims the defined digitised corpus did not establish. |
| Research significance | Methodological significance of the case. |
| Notes | Implementation and production-verification notes. |

## Interpretation

The matrix is an audit trail rather than a scorecard. It records what was retrieved, what was inferred and where the evidence stopped. A positive provenance check does not by itself establish that a historical interpretation is correct.

The matrix should be read alongside `experiment/research_questions.csv`, `experiment/retrieval_routes.md` and `experiment/evaluation_protocol.md`.
