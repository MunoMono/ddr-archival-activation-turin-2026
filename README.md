# DDR archival activation–Turin 2026

Supplementary research artefact for Graham Newman's 2026 conference paper on archival activation, synthetic heritage, retrieval-augmented inference and scoped missingness in the Royal College of Art's Department of Design Research (DDR) archive.

## Purpose

This repository preserves the evidence package behind the reported 12-case experiment. It is intended to keep the paper's research design, findings matrix, prompt set, provenance material and selected visual documentation inspectable without overloading the conference paper itself.

The repository should be read as a research artefact, not as a digital surrogate for the complete DDR archive. The experimental evidence surface is partial and bounded. Some DDR material remains undigitised, image-only, unavailable or insufficiently described.

## Experimental scope

The experiment used a corpus of 27,997 PID-backed text chunks. Questions were selected purposively as stress tests rather than as a representative sample of DDR history.

The 12 cases are grouped into:

1. **Known relationships**–retrieval across people, projects and activities while keeping archival association, documentary attribution and inferred responsibility distinct.
2. **Contested interpretations**–comparison of different formulations, voices, source types and temporal positions without turning recurrence into consensus or variation into documented disagreement.
3. **Scoped missingness**–retrieval of the nearest relevant traces while stating where the defined evidence surface does not establish the stronger historical claim.

The live research instrument uses two local models with separate functions: Qwen3 8B as a bounded inference layer and BAAI bge-m3 for semantic embeddings and retrieval. The same embeddings also support UMAP-based visual analytics.

## Repository structure

```
data/
  known_relationships.csv
  contested_interpretations.csv
  scoped_missingness.csv
  data_dictionary.md

experiment/
  research_questions.csv
  retrieval_routes.md
  evaluation_protocol.md

figures/
  README.md

uat/
  known-relationships/
  contested-interpretations/
  scoped-missingness/

provenance/
  README.md

supplementary/
  README.md
```

## Evidence and interpretation

Retrieved passages retain document and chunk identifiers, source metadata and provenance. Documentary text, archival or authority metadata and later oral testimony are kept distinct throughout the workflow.

The experiment evaluates whether retrieval returns relevant traces, whether responses preserve evidential status, whether ambiguity is retained and whether the system recognises where the available evidence stops.

Three CSV files contain the complete 12-case findings matrix, one for each experimental cluster. They preserve all fields from the working findings matrix: what retrieval surfaced, what the model inferred, what proved useful, what was overstated or flattened, what the corpus did not establish and why each case matters.

## Rights and source material

This repository does **not** grant permission to reproduce archival source material held by the Royal College of Art, the Victoria and Albert Museum or other rights holders. See [RIGHTS.md](RIGHTS.md).

Source scans, photographs and high-resolution archival images should only be added where their reproduction rights permit public redistribution.

## Citation

Citation metadata is provided in [CITATION.cff](CITATION.cff). A DOI can be added after an archival release is deposited with a service such as Zenodo.

## Status

This repository is a working scholarly supplement for the Turin 2026 conference paper. The paper, figures and supporting material remain subject to revision until the conference-paper release is frozen.
