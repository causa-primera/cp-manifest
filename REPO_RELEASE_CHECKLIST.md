# REPO_RELEASE_CHECKLIST.md

Use this checklist before publishing any release `vX.Y.Z` in any Causa Primera repository.

## A) Baseline repository health (mandatory)
- [ ] Default branch is `main`
- [ ] `LICENSE` exists (text repos: CC BY 4.0)
- [ ] `RIGHTS.md` exists (VoR policy stated)
- [ ] `CITATION.cff` exists and matches repo name + URL
- [ ] `CHANGELOG.md` updated for `vX.Y.Z`
- [ ] `README.md` exists and points to core artifacts
- [ ] (If AI contributed materially) `AI_CONTRIBUTION_LOG.md` updated

## B) Model B provenance (mandatory)
- [ ] Spanish snapshot folder exists: `es-snapshots/vX.Y.Z/`
- [ ] Snapshot includes (minimum):
  - [ ] `THESIS.es.md`
  - [ ] `ARGUMENT_MAP.es.md`
  - [ ] `GLOSSARY.es.md`
- [ ] Snapshot is treated as frozen after release (no edits)
- [ ] `TERMINOLOGY.md` exists (controlled vocabulary)
- [ ] `TRANSLATION_POLICY.md` exists
- [ ] `TRANSLATION_LOG.md` has an entry for `vX.Y.Z`
- [ ] Any conceptual mismatch is logged as **Substantive divergence** (no silent divergence)

## C) Gate compliance (select what applies)
### Core Gate v0.1.0 (Scaffold)
- [ ] `THESIS.en.md`
- [ ] `ARGUMENT_MAP.en.md`
- [ ] `GLOSSARY.en.md`
- [ ] (Core-03) `INVARIANTS.en.md`

### Core Gate v0.3.0 (Core solidity)
- [ ] `OBJECTIONS.en.md` (>=10, steelman)
- [ ] `RESPONSES.en.md` (paired to objections)
- [ ] `INVARIANTS.en.md` (>=5)
- [ ] `TESTS.en.md` (>=6)
- [ ] Glossary has >=20 terms and boundary notes
- [ ] Argument map uses numbered premises and glossary dependencies

### Domain Gate v0.2.0
- [ ] `BRIDGE_TO_CORE.en.md`
- [ ] `FRICTIONS.en.md` (>=2)
- [ ] `RESULT.en.md` (>=1 novel result)
- [ ] `COMPATIBILITY.md` declares minimum core versions

## D) Release packaging (GitHub Releases)
- [ ] Create/choose tag `vX.Y.Z` (SemVer)
- [ ] Release title is `vX.Y.Z`
- [ ] Release notes include:
  - [ ] What changed
  - [ ] What is new
  - [ ] Known limitations
  - [ ] Pointer to `es-snapshots/vX.Y.Z/`
- [ ] Publish release
