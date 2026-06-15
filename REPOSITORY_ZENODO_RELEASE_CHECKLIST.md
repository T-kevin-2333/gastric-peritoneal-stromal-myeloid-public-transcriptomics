# Repository and Zenodo release checklist

## Completed decisions

- GitHub owner: `T-kevin-2333`.
- Repository: `gastric-peritoneal-stromal-myeloid-public-transcriptomics`.
- Visibility: public.
- Code/scripts license: MIT.
- Non-code derived materials license: CC BY 4.0.
- Authors approved public repository release.
- Raw public data and restricted patient-level data are not redistributed.

## GitHub release sequence

1. Confirm the complete ZIP is present in the repository.
2. Create tag: `v0.1.0-submission`.
3. Create GitHub release using `GITHUB_RELEASE_NOTES_DRAFT.md`.

## Zenodo sequence

1. Link Zenodo to the GitHub repository.
2. Archive the GitHub release `v0.1.0-submission`.
3. Copy the final Zenodo DOI.
4. Replace manuscript placeholders using `DATA_AVAILABILITY_REPLACEMENT_DRAFT.md` or `scripts/104A_apply_repository_zenodo_urls.py`.

## Do not do

- Do not invent a Zenodo DOI before deposition.
- Do not submit `<RECORD_ID>` placeholders to the journal.
- Do not claim raw public data are hosted in the repository.
