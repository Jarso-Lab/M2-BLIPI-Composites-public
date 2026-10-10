# M2-BLIPI Composites

### Do biologically motivated metabolic scores carry prognostic information in Burkitt lymphoma?

This repository is the public home of the composite-score study within the M2-BLAIPI
research program at Johns Hopkins University. It currently describes the project only.
**Code and data are not released yet and will be made available when the research is
published.**

---

## Background

Burkitt lymphoma (BL) is an aggressive B-cell malignancy and a major cause of childhood
cancer mortality in malaria-endemic regions of sub-Saharan Africa. The Burkitt Lymphoma
International Prognostic Index (BL-IPI) estimates risk from clinical variables alone, so it
cannot reflect the biological differences between tumors. Genomic studies have shown that BL
divides into distinct genetic subgroups (DGG-BL, IC-BL, Q53-BL) with different oncogenic
drivers, and tumor metabolism is one downstream layer where that biology becomes measurable.

The M2-BLAIPI program asks whether metabolic pathway activity, inferred from gene expression
and anchored to genomic subgroups, adds prognostic signal beyond the clinical baseline.

## This study

A central idea of the program is to summarize driver-linked metabolic biology as
literature-derived **composite metabolic scores**: compact, interpretable features built from
gene-expression pathway activity. Before scores like these can support any risk model, they
have to be shown to be trustworthy. This study tests them directly.

### Aims

1. **Rigorous internal validation.** Determine, with bias-corrected internal validation and
   formal equivalence testing, whether the composite scores add prognostic information beyond
   the clinical index, and whether the available sample is large enough to detect a
   clinically meaningful gain.
2. **Independent, correctly signed information.** Determine whether each score contributes
   to a survival model that already contains a reference panel of established pathway
   measures, and whether its direction of effect matches the biology it was designed to
   capture.
3. **Limits of generalization.** Characterize how far the scores and the associated model can
   be carried to other cohorts, given the clinical information that public BL cohorts
   actually record.

### Approach (high level)

- Publicly accessible BL genomic, transcriptomic, and clinical data, accessed under the terms
  of the originating cohorts.
- Sample-level pathway activity inferred from gene expression with Gene Set Variation
  Analysis (GSVA).
- Survival modeling evaluated with nested cross-validation, with every data-dependent step
  fitted inside the training folds, and benchmarked against a clinical-variable-only
  baseline.
- Analyses stratified by EBV status to separate subgroup-associated signals from
  EBV-associated ones.

Results are not reported here until they have been peer reviewed.

## Relationship to M2-BLAIPI

M2-BLAIPI is the broader research program, whose long-term goal is a biologically informed
risk score for Burkitt lymphoma. This repository covers the composite-score study only.
Other parts of the program are maintained in separate repositories.

## Data

No patient-level data are, or will be, distributed in this repository. All cohorts are
de-identified and used under their originating Data Use Agreements; anyone reproducing the
work will obtain the data from the original sources.

## Citing

Citation metadata are in [CITATION.cff](CITATION.cff). A full reference will be added on
publication.

## Contact

Samson Jarso, PhD, Applied Biomedical Engineering, Johns Hopkins University.
