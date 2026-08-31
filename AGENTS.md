# AI / Contributor Guide

This is a large legacy slicer codebase/fork. Favor conservative, well-scoped changes and upstream compatibility over broad rewrites.

## Priorities
1. Do not add runtime AI to slicing, geometry, toolpath, or machine-control logic without a separate design, reproducible benchmarks, and human review.
2. AI may assist development, documentation, test generation, issue triage, or explaining settings, but must not silently alter safety-critical print parameters.
3. Preserve compatibility with existing file formats, profiles, and command-line behavior unless a change is explicitly documented.
4. Never commit secrets, private printer credentials, or user models.
5. Add regression tests for geometry/toolpath changes.
6. Keep platform-specific build behavior in mind and avoid unnecessary dependency churn.
7. Prefer small commits that can be compared with upstream.
8. Document deviations from upstream and any migration requirements.

## Before merging
- Run the relevant test/build targets.
- Compare generated output for representative models when slicing behavior changes.
- Check backward compatibility with existing profiles/configs.
- Review for accidental large-formatting/vendor changes.
