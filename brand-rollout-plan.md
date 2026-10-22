# Clinical Registry unified brand rollout

Status: draft implementation plan; user authorized build and deployment on 2026-10-22.

Issue: https://github.com/justin-napolitano/clinical-registry-data-platform-site/issues/1

## Context and scope

This static HTML showcase owns public registry documentation. Use the approved `08-index-simplified-no-marks.png` reference and pinned shared contract from littlelink planning PR #30. Preserve existing source content, registry coverage, tables, links, technical diagrams and routes. Update only presentation and accessibility semantics related to responsive reading; do not change access controls, data or external integrations. No image/logo character precedes any site title.

## Plan of work

1. Capture existing static routes and presentation, and make isolated initiative/implementation branches.
2. Use locally served Inter and Source Serif 4 fonts with OFL notices. Apply warm paper/ink/stone with restrained slate; modest title size, thin dividers, simple horizontal navigation and square editorial surfaces. Remove the huge hero and decorative gradient/card styling while keeping useful content.
3. Make existing data tables keyboard-accessible scroll regions; retain full metadata and original destinations.
4. Check every local HTML/CSS/font link; verify no facts were changed. Serve locally and inspect desktop/mobile, overflow, focus and contrast before deployment.
5. Commit and publish the scoped PR with evidence. Preserve a known previous deployment for rollback; publish through the existing verified hosting project after visual/build checks. Record production URL, commit and smoke results.

## Validation and acceptance

No package build exists. Validate static references and semantic structure, all 18 HTML routes, font licenses and source scope. Browser checks at 390/768/1440px plus 320px overflow, keyboard navigation and content table scrolling. Browser fallback authorization is pending; do not mark visual QA passed without rendered evidence. Deployment awaits valid existing hosting credentials and a known project/domain mapping. Use only already-public content in evidence. No patient data is introduced.

## Recovery

Revert the focused presentation commit or restore the recorded previous production deployment. No migration, data changes, credential changes, domain activation or DNS changes are included.
