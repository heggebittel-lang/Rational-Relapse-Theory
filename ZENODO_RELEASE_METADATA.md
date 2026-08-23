# Zenodo Release Metadata Queue

This file records the intended metadata sequence for the unreleased archive versions v4.0–v9.0. The root `.zenodo.json` should describe the **next release to be created**, and should be advanced to the next block before creating the next GitHub tag/release.

Do not create all six tags first and edit metadata afterward: Zenodo archives the repository state associated with each release.

## Release order

1. `v4.0`
2. `v5.0`
3. `v6.0`
4. `v7.0`
5. `v8.0`
6. `v9.0`

## v4.0

**Title:** Rational Relapse Theory Archive v4.0: Axiomatic Endogenous-Recovery Structural Model  
**Historical label:** v6.2  
**Primary language:** Chinese; English archival companion included  
**Suggested keywords:** rational addiction; endogenous recovery; target stock; dynamic choice; bifurcation; research archive

Description: archival release of the June 2026 manuscript stage originally labeled v6.2. It develops an axiomatic endogenous-recovery structural model within rational addiction. The historical Chinese manuscript is authoritative for this stage; the English version is an archival translation/reader.

## v5.0

**Title:** Additive Measurement on Path-Generated Domains: Directed Recovery in Rational Addiction  
**Historical label:** JME-S-26-00480  
**Languages:** English + Chinese archival translation  
**Suggested keywords:** additive measurement; path-generated domains; finite cancellation; Stieltjes representation; directed recovery; rational addiction

Description: archival release of the path-generated-domain stage. The paper shifts the primitive object from a recovery utility function to target-relative continuous paths and accessible ledgers, and studies a finite-cancellation/Stieltjes-representation route. Rational addiction is treated as the leading economic application.

## v6.0

**Title:** Recovery Histories: Exact Passage Compression and Additive Choice  
**Historical label:** JET_Recovery_Histories_v25  
**Languages:** English + Chinese archival translation  
**Suggested keywords:** recovery histories; passage compression; additive choice; path fibers; Stieltjes representation; measurement

Description: archival release of the recovery-histories stage. It develops exact passage compression, path-fiber arguments, balance/cancellation conditions, and an additive/Stieltjes representation on the compressed history domain.

## v7.0

**Title:** Revealed Reinforcement and Recovery Value: Compensated Choice under State-Dependent Valuation  
**Historical label:** JME-D-26-00519  
**Languages:** English + Chinese archival translation  
**Suggested keywords:** compensated choice; revealed reinforcement; recovery value; state-dependent valuation; identification; revealed preference

Description: archival release of the two-experiment compensated-choice stage. Binary monetary compensation identifies marginal revealed valuation; a second recovery experiment is used to study a common state-dependent value geometry and local recovery sensitivity.

## v8.0

**Title:** Compensated Choice and Recursive Counterfactual Identification  
**Historical label:** recursive_monetary_comparison_core_theory_v9_1  
**Languages:** English + Chinese archival translation  
**Suggested keywords:** compensated choice; recursive identification; transition matching; index propagation; counterfactual comparative statics; revealed preference

Description: archival release of the recursive counterfactual-identification stage. The surviving English PDF is the authoritative historical artifact because the original LaTeX source was lost. A reconstructed English source and Chinese archival translation are preservation aids and are explicitly labeled as such.

## v9.0

**Title:** Compensated Current Choice and Counterfactual Identification  
**Historical label:** Compensated_Current_Choice_v38_Economic_Grounding  
**Languages:** English + Chinese archival translation  
**Suggested keywords:** compensated current choice; counterfactual identification; continuation information; finite differences; cycle space; comparative statics

Description: archival release and current endpoint of the research program. Standard compensated-choice, cancellation, graph/cycle-space, finite-difference, and dynamic tools are treated as background infrastructure. The substantive question is the comparison support and information structure needed to identify a counterfactual local choice response.

## After each Zenodo deposit

After Zenodo assigns the version DOI:

- add the DOI to that version's `README.md`;
- replace `DOI pending release` in the root `README.md`;
- update `ARCHIVE_INDEX.md`;
- optionally add the DOI to the release notes;
- then advance `.zenodo.json` to the metadata block for the next version **before** creating the next GitHub Release.
