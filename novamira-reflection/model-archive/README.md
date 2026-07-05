# Novamira Reflection Public Artifacts

This directory is a public-artifact staging area for Novamira reflection.

## Source of truth

- These files are not the HaruHP source of truth.
- The source of truth remains the private HaruHP repository, especially `templates/` and `generated/wordpress/`.
- This artifact lane exists so WordPress/Novamira can fetch long HTML/CSS without credentials.
- Replace `PUBLIC_ARTIFACT_BASE_URL` with the final public artifact URL after publishing this directory to a public repository or GitHub Pages.

## Safety policy

- WordPress updates must only happen after LF length and SHA256 verification.
- Published pages are `compare_only` and must not be directly updated by this workflow.
- Future real update candidates must be draft `post_content` targets.
- `custom_css` remains `compare_only_until_explicit_approval` because it is site-wide.
- Global Styles / `wp_global_styles` / post_id 17 are out of scope.
- No GitHub token, Application Password, or WordPress credential belongs in this artifact.

## Included files

- `wp-reflection-manifest.json`: manifest with target definitions, source private repo commit, public artifact URL placeholders, length, SHA256, and update policy.
- `model-archive-body.html`: generated WordPress body HTML for Model Archive comparison.
- `model-archive-additional.css`: generated WordPress additional CSS for Model Archive comparison.

## Current manifest summary

- Source private repo commit: `f82c9916ae5231920a310ebef218cc601fc09620`
- Generated at: `2026-07-05T14:26:49+00:00`
- Update policy: `draft_only`
- Published post policy: `compare_only`
- Custom CSS policy: `compare_only_until_explicit_approval`
