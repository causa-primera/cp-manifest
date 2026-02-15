# TRANSLATION_CHECKLIST.md (Model B)

This checklist enforces: English canonical track + Spanish frozen provenance snapshots.

## 1) Freeze Spanish snapshot (pre-release)
- [ ] Create folder: `es-snapshots/vX.Y.Z/`
- [ ] Add frozen Spanish artifacts (minimum):
  - [ ] `THESIS.es.md`
  - [ ] `ARGUMENT_MAP.es.md`
  - [ ] `GLOSSARY.es.md`
- [ ] Confirm snapshot will not change after release (treat as immutable)

## 2) Produce English canonical artifacts
- [ ] Update:
  - [ ] `THESIS.en.md`
  - [ ] `ARGUMENT_MAP.en.md`
  - [ ] `GLOSSARY.en.md`
- [ ] Update repo-specific gate artifacts (tests/invariants/objections, if relevant)

## 3) Terminology control
- [ ] Update `TERMINOLOGY.md` for new or revised terms
- [ ] Ensure glossary usage matches controlled vocabulary constraints

## 4) Translation policy + log
- [ ] `TRANSLATION_POLICY.md` unchanged unless explicitly amended
- [ ] Add `vX.Y.Z` entry in `TRANSLATION_LOG.md`:
  - [ ] Summary of translation decisions
  - [ ] Terminology changes
  - [ ] **Substantive divergences** (if any), each with:
    - EN change description
    - ES snapshot reference
    - justification
    - scope/impact

## 5) Final consistency checks
- [ ] No silent conceptual differences EN vs ES
- [ ] `CHANGELOG.md` updated for `vX.Y.Z`
- [ ] Release notes drafted and include link/pointer to `es-snapshots/vX.Y.Z/`
