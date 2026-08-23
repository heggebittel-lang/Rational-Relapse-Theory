# Release Readiness Checklist

This file records the completed archival release sequence for v4.0–v9.0. The goal was to preserve the authoritative historical PDFs, bilingual companions where prepared, provenance notes, checksums, and version-specific Zenodo citation objects without forcing cosmetic symmetry across all historical folders.

## Minimum release standard

A version was treated as release-ready when the repository contained:

1. the authoritative historical PDF;
2. the Chinese or English companion PDF when one had been prepared;
3. a version `README.md` explaining manuscript identity and translation/reconstruction status;
4. `PRIORITY_AND_PROVENANCE.md`;
5. `RELEASE_NOTES.md`;
6. an integrity record matching the files intended for release.

LaTeX sources and figure files were treated as recommended preservation assets rather than DOI-blocking requirements when the authoritative PDFs and provenance record were already present.

## Final status

| Version | Authoritative PDF | Companion PDF | Provenance | Integrity record | Status |
|---|---:|---:|---:|---:|---|
| v4.0 | Chinese PDF present and verified | English PDF present and verified | yes | verified | **released — DOI 10.5281/zenodo.22067123** |
| v5.0 | English PDF present | Chinese PDF present | yes | verified | **released — DOI 10.5281/zenodo.22067231** |
| v6.0 | English PDF present | Chinese PDF present | yes | verified | **released — DOI 10.5281/zenodo.22067292** |
| v7.0 | English PDF present | Chinese PDF present | yes | verified | **released — DOI 10.5281/zenodo.22067412** |
| v8.0 | surviving English PDF present | Chinese PDF present | yes; source-loss note explicit | standardized | **released — DOI 10.5281/zenodo.22067461** |
| v9.0 | English endpoint PDF present | Chinese PDF present | yes | verified | **released — DOI 10.5281/zenodo.22067526** |

## Version-specific Zenodo rule

The GitHub repository preserves the complete v1.0–v9.0 research history, while each Zenodo citation object for v4.0–v9.0 contains only the archive folder for the corresponding stage. This avoids using a whole-repository snapshot as the primary citation object for an individual historical manuscript.

## Non-blocking preservation assets

Additional source files and figures may remain in the repository or in release packages for reproducibility. Their presence is archival support and does not reopen the theoretical content. In particular, the v8.0 surviving PDF remains the authoritative historical English artifact; reconstructed source material is labeled accordingly.

## Completion

The v4.0–v9.0 GitHub Release → Zenodo DOI sequence is complete. Together with the earlier v1.0–v3.0 records, all nine archive stages now have persistent DOI citations.

Future changes that materially alter a released manuscript should receive a new archive/release version rather than silently replacing the existing DOI object.
