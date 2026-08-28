# Awesome Token-Level Uncertainty

A curated academic resource collection on **token-level uncertainty as a predictor of hallucination in Large Language Models (LLMs)**. It connects the supplied AI-assisted research paper with verified scholarly literature, hallucination/factuality benchmarks, uncertainty-estimation tools, reproducible implementations, and learning resources. The collection emphasizes the distinction between lexical/token uncertainty and semantic uncertainty, as well as calibration, evaluation, and practical hallucination detection.

## Contents
- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Citation Integrity Audit](#citation-integrity-audit)
- [Claim-Citation Audit](#claim-citation-audit)
- [Survey and Review Papers](#survey-and-review-papers)
- [Foundational and Calibration Papers](#foundational-and-calibration-papers)
- [Token and Semantic Uncertainty](#token-and-semantic-uncertainty)
- [Hallucination and Factuality Evaluation](#hallucination-and-factuality-evaluation)
- [Mitigation and Verifiability](#mitigation-and-verifiability)
- [Datasets and Benchmarks](#datasets-and-benchmarks)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Tutorials and Learning Resources](#tutorials-and-learning-resources)
- [License](#license)

## Overview

Large Language Models generate text token by token from probability distributions over a vocabulary. This makes token-level probabilities, entropy, and related uncertainty measures attractive intrinsic signals for estimating whether a generation is reliable. However, token uncertainty does not automatically equal uncertainty about the underlying meaning: a correct answer can have several valid phrasings, while an incorrect semantic claim can sometimes be generated with high confidence.

Research therefore spans several connected directions. Token-level methods such as Claim Conditioned Probability attempt to isolate uncertainty about factual claims from surface-form variation. Semantic-entropy methods instead compare the meanings of multiple sampled answers, while newer approaches such as Semantic Entropy Probes, uncertainty heads, and length-invariant uncertainty corrections aim to obtain useful semantic or reliability signals more efficiently. Calibration is another central issue because raw confidence can be systematically misaligned with actual correctness.

The collection below organizes the literature around these themes and connects them to datasets and benchmarks for hallucination/factuality evaluation. It also includes practical tools and implementations so that a reader can move from the theory of uncertainty estimation to reproducible experiments and evaluation.

## AI-Assisted Research Paper

**Token-Level Uncertainty as a Predictor of Hallucination in Large Language Models**

The supplied paper reviews token-level uncertainty, semantic entropy, Claim Conditioned Probability (CCP), Semantic Entropy Probes (SEPs), Calibrated Entropy Scores (CES), and pre-trained uncertainty-quantification heads. It also discusses calibration, computational cost, layer-specific effects, multi-step reasoning, and future directions.

**[View the AI-Assisted Research Paper](paper/AI_Assisted_Research_Paper.pdf)**

## Citation Integrity Audit

A citation/resource audit was prepared to verify the references appearing in the supplied paper and to document the verification rules used for the curated collection.

**[View the Citation Integrity Audit PDF](citation-audit/Citation_Integrity_Audit.pdf)** · **[View the audit notes](citation-audit/audit.md)**

The claim-level review is available in **[claim_citation_audit.md](citation-audit/claim_citation_audit.md)**. It explicitly flags claims in the supplied paper that depend on the incomplete Villani reference.

## Claim-Citation Audit

The repository distinguishes reference verification from claim verification. Major claims in the supplied paper were reviewed against their cited sources; claims depending on the incomplete Villani reference are explicitly marked as requiring correction/verification.

## Survey and Review Papers

See the complete metadata, links, and relevance notes in **[references/references.md](references/references.md)**.

- Survey of Hallucination in Natural Language Generation
- A Survey on Hallucination in Large Language Models

## Foundational and Calibration Papers

See **[references/references.md](references/references.md)** for full author lists and direct paper/DOI links.

- On Calibration of Modern Neural Networks
- Simple and Scalable Predictive Uncertainty Estimation using Deep Ensembles
- Language Models (Mostly) Know What They Know
- TruthfulQA: Measuring How Models Mimic Human Falsehoods

## Token and Semantic Uncertainty

These papers are closest to the assigned research topic.

- Fact-Checking the Output of Large Language Models via Token-Level Uncertainty Quantification
- Detecting Hallucinations in Large Language Models Using Semantic Entropy
- Semantic Entropy Probes: Robust and Cheap Hallucination Detection in LLMs
- On Subjective Uncertainty Quantification and Calibration in Natural Language Generation
- UNCERTAINTY-LINE: Length-Invariant Estimation of Uncertainty for Large Language Models
- A Head to Predict and a Head to Question: Pre-trained Uncertainty Quantification Heads for Hallucination Detection in LLM Outputs

Full entries are in **[references/references.md](references/references.md)**.

## Hallucination and Factuality Evaluation

- SelfCheckGPT
- HaluEval
- FActScore
- TRUE
- RAGTruth
- FELM
- Evaluating Verifiability in Generative Search Engines
- Enabling Large Language Models to Generate Text with Citations

**[Browse the verified paper collection](references/references.md)**.

## Mitigation and Verifiability

- RARR
- Chain-of-Verification
- DoLa
- TruthX

These methods complement uncertainty-based detection by addressing attribution, verification, decoding, or representation-level mitigation.

## Datasets and Benchmarks

The assignment requires at least three relevant datasets/benchmarks. This repository includes five.

**[Open the complete dataset/benchmark list](datasets/datasets.md)**

Included: HaluEval, RAGTruth, TruthfulQA, ALCE, and FELM.

## Tools and Libraries

The repository includes six relevant tools/resources.

**[Open the complete tools list](tools/tools.md)**

Included: LM-Polygraph, Semantic Uncertainty, UQ-NLG, Ragas, SelfCheckGPT, and UNCERTAINTY-LINE.

## GitHub Implementations

The implementations section considers documentation, source availability, maintenance/activity, reproducibility, licensing, and connection to research—not popularity alone.

**[Open the complete implementation list](implementations/github-repositories.md)**

Included: SelfCheckGPT, Semantic Uncertainty, LM-Polygraph, ALCE, TruthX, and RAGTruth.

## Tutorials and Learning Resources

**[Open the complete learning-resource list](tutorials/tutorials.md)**

Included: Stanford CS336, Stanford CS336 lecture repository, LM-Polygraph, Ragas documentation, ALCE reproduction resources, and SelfCheckGPT project resources.

## Verification and Ethical Use

- Scholarly metadata was checked against authoritative records before inclusion.
- Third-party research PDFs are **not** bundled in this repository.
- The supplied AI-assisted paper is included because it is the student's own assignment artifact.
- The uncertain Villani reference in the supplied paper is explicitly flagged in the audit and is not counted toward the verified-paper minimum.
- External resources remain subject to their own licenses and terms.

## License

The repository's original documentation and curation files are released under the **MIT License**. Third-party resources linked from this repository retain their respective licenses.

See **[LICENSE](LICENSE)**.
