# Release Readiness Checklist

This checklist separates the **minimum archival record** needed before creating each GitHub Release from optional source material. The goal is to avoid delaying the DOI sequence for cosmetic symmetry.

## Minimum release standard

A version is release-ready when the repository contains:

1. the authoritative historical PDF;
2. the Chinese or English companion PDF when one has been prepared;
3. a version `README.md` explaining manuscript identity and translation/reconstruction status;
4. `PRIORITY_AND_PROVENANCE.md`;
5. `RELEASE_NOTES.md`;
6. `SHA256SUMS.txt` matching the files intended for release.

LaTeX sources and figure files are recommended preservation assets, but they are not required for the DOI sequence if the authoritative PDFs and provenance record are already present.

## Current status

| Version | Authoritative PDF | Companion PDF | Provenance | Checksums | Status |
|---|---:|---:|---:|---:|---|
| v4.0 | **missing from repository** (original Chinese PDF) | English PDF present | yes | yes | **one blocking file remains** |
| v5.0 | English PDF present | Chinese PDF present | yes | corrected to uploaded PDFs | ready for final review |
| v6.0 | English PDF present | Chinese PDF present | yes | matches uploaded PDFs | ready for final review |
| v7.0 | English PDF present | Chinese PDF present | yes | matches uploaded PDFs | ready for final review |
| v8.0 | surviving English PDF present | Chinese PDF present | yes; source-loss note explicit | standardized | ready for final review |
| v9.0 | English endpoint PDF present | Chinese PDF present | yes | corrected to uploaded PDFs | ready for final review |

## v4.0 blocking item

Before creating the `v4.0` GitHub Release, add the original Chinese historical manuscript as:

`v4.0/v4.0.pdf`

Its prepared SHA-256 is recorded in `v4.0/SHA256SUMS.txt`. The English companion `v4.0_en.pdf` is already present.

## Recommended, non-blocking source preservation

When convenient, the following source files can also be committed or attached to the corresponding release:

- v4.0: original Chinese TeX, English companion TeX, fold and Neimark–Sacker illustrations;
- v5.0: English and Chinese TeX plus the three historical figures and graphical abstract;
- v6.0: original English source, Chinese source, path-accounting figures and bibliography;
- v7.0: English/Chinese sources, five figures and graphical abstract;
- v8.0: reconstructed English source and Chinese source, always labeled as reconstructed/translation material;
- v9.0: English source and the four final figures; Chinese source is already represented in the repository.

These additions improve reproducibility but should not reopen the theoretical content.

## Release sequence

Once v4.0 has its original Chinese PDF, proceed sequentially:

`v4.0 → Zenodo DOI → update metadata → v5.0 → ... → v9.0`

Before each release, advance the root `.zenodo.json` using [`ZENODO_RELEASE_METADATA.md`](./ZENODO_RELEASE_METADATA.md). After Zenodo assigns a DOI, update the version README, root README, and [`ARCHIVE_INDEX.md`](./ARCHIVE_INDEX.md) before moving to the next version.
