# Novamira Subject Archive Public Artifact

This directory holds draft preparation artifacts for Misaki / Yui Subject Archive pages.

## Files in this directory

- `wp-reflection-manifest.json`: draft-lane-only manifest for Subject Archive candidates
- `irontechdoll-158cm-a4-misaki-silk-glow.html`: source WordPress body HTML for Misaki subject archive
- `irontechdoll-158t-a5-ros-max-yui-silk-glow.html`: source WordPress body HTML for Yui subject archive

## Rules for this prepare artifact set

- Source files are local private-repo generated HTML from `generated/wordpress/subjects/`.
- This set is **prepare-only** and does not grant update or create execution.
- `create_allowed` and `update_allowed` are explicitly `false` in the manifest.
- `public_artifact_base_url` is placeholder-driven and must be replaced after this directory is published to a public artifact repository.
- `required_status` is `absent_or_draft` so only safe draft-creation preparation is recorded.

## Prohibitions to keep this set read-only

- No WordPress publish.
- No delete.
- No URL or slug changes.
- No `wp_insert_post`.
- No `wp_update_post`.
- No `wp_update_custom_css_post`.
- No `wp_global_styles` operations.
- No WordPress update execution in this step.
- No public repository push in this step.
- No credentials are stored in this directory.
