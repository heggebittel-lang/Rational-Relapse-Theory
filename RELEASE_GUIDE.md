# GitHub Release and Zenodo Guide

The repository is organized so that each historically meaningful manuscript can receive a separate GitHub Release and, through Zenodo's GitHub integration, a separate archival DOI.

## Planned release sequence

- **v4.0** — Axiomatic endogenous-recovery structural model (original internal label: v6.2)
- **v5.0** — Additive Measurement on Path-Generated Domains: Directed Recovery in Rational Addiction
- **v6.0** — Recovery Histories: Exact Passage Compression and Additive Choice
- **v7.0** — Revealed Reinforcement and Recovery Value: Compensated Choice under State-Dependent Valuation
- **v8.0** — Compensated Choice and Recursive Counterfactual Identification
- **v9.0** — Compensated Current Choice and Counterfactual Identification

## Recommended workflow for each release

1. Confirm that the version folder identifies the exact manuscript intended for preservation, including its original internal/submission label and date where known.
2. Record a SHA-256 checksum for every PDF/source file that will be released. Commit the checksum file before or together with the archival release.
3. For v4.0, preserve the Chinese original and make the English reader/companion clearly identifiable as a translation of the same historical stage.
4. Create a GitHub Release with the matching tag (`v4.0`, `v5.0`, …).
5. Attach the exact release files individually (PDF, source, figures, checksum file) so that readers and Zenodo can preserve the scholarly object directly rather than only through a bundled ZIP.
6. Use the manuscript title as the release title and identify the original internal/submission label in the release notes.
7. Let Zenodo archive the GitHub release.
8. After Zenodo assigns the DOI, add that DOI to the version README and the root version table.
9. Verify the downloaded archival files against the committed SHA-256 checksums.
10. Do not silently replace a released PDF with a materially different manuscript. Use a new release/version when the scholarly object changes materially.

## Provenance and priority

A dated source file, a public Git commit, a GitHub Release, cryptographic hashes, and a Zenodo deposit together form a useful provenance chain. They can document what exact scholarly object existed by a particular date and make later comparison straightforward.

A DOI is useful for persistent identification, citation, and timestamped preservation, but it is not itself a legal determination of authorship, copyright ownership, patent rights, or priority. Preserve original source files, dated drafts, submission correspondence, and release history where available.

## Copyright and licensing

Copyright protection and licensing are different questions from DOI registration. A repository license states what permissions are granted to downstream users; a DOI does not make a permissively licensed work exclusive. Before releasing a version, check that the repository/version license reflects the permissions the author actually wants to grant. Do not assume that a later license change can withdraw permissions already granted for copies previously distributed under an earlier license.

## Metadata discipline

The archive version number is intentionally simple. The original filename or journal-submission number is retained in each folder so that older correspondence can be matched unambiguously to the archived paper.

Before each Zenodo-synchronized release, check that title, author, ORCID, description, license, version, publication date, and related identifiers describe the manuscript being released rather than a later version of the project.
