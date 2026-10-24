# Brand design QA

Source visual truth: `/Users/justin/repos/brand-review/2026-10-22/08-index-simplified-no-marks.png` (1448×1086). Approved multi-site brand board; the real product's copy/routes/content are retained, so this is a style comparison rather than invented pixel equality with a placeholder panel.

Implementation screenshots: `/Users/justin/repos/brand-review/2026-10-22/implementation-evidence/browser-qa/2026-10-22T19-08-00-475Z/registry-{390,768,1440,320}.png`.
Full-view combined comparison: `/Users/justin/repos/brand-review/2026-10-22/implementation-evidence/browser-qa/2026-10-22T19-08-00-475Z/registry-comparison.png`.
Focused article/table/reader combined reference comparison: `/Users/justin/repos/brand-review/2026-10-22/implementation-evidence/root-detail-qa/registry-comparison.png`; raw focused screenshots and `checks.json` are alongside it. Source and actual screenshots were rendered together in one comparison image and opened for review.

Viewport/density: 390/768/1440×900 CSS px, deviceScaleFactor1; additional320px narrow-screen and720px effective200% reflow checks. Comparison images label their scaled source/desktop/mobile sizes. Effective reflow is not a claim of native browser toolbar zoom. No page-level horizontal overflow was found. Writing-site local builds override only base URL to loopback; release configuration and domains are unchanged.

State and interactions: Home, coverage table, metadata and pipeline routes; all 18 local HTML links checked. Named focusable table scroll region and keyboard focus verified.

Required fidelity surfaces reviewed:
- Fonts/type: locally hosted Inter UI and Source Serif4 reading hierarchy, modest24–28px headings, no prefixed title character. Print uses its separate readable export settings.
- Spacing/layout: restrained rules, usable navigation, readable wrapping and consistent gutters; no giant hero or hidden persistent control.
- Colors: warm paper/ink, stone rules, restrained accessible slate links; no large blue treatment. Visible keyboard focus retained.
- Assets: no decorative photography added; existing meaningful content imagery/code is preserved. Local licensed font assets load.
- Copy: real source material retained, no board placeholder claims inserted.

Findings and comparison history: No actionable P0/P1/P2 differences. Technical tables use local horizontal scrolling rather than removing columns.

Console: no page JavaScript exception. Registry/writing public routes have no failed resources in the final local run. News's deliberately disconnected graph preferences endpoint is recorded above rather than counted as a successful integration.

Implementation checklist: responsive captures reviewed; reference comparisons opened; focused states tested; applicable fixes recaptured. No remaining actionable P0/P1/P2 visual finding. Existing external integrations and live authentication will be checked read-only after deployment without changing protection.

final result: passed


## 2026-10-23: Shared midpoint palette

Final result: passed

Apply midpoint red (#d01527) to text accents, hover/focus/selection states, keeping green (#356349) exclusively as the native scroll canvas behind a full-height paper page surface. Screen-only overrides preserve print styling and published PDF files. Existing dark modes retain readable contrast with a lighter red text variant. No application data, destinations, authentication, or runtime dependencies changed.

The production build/static checks pass using the repository lockfile. Browser checks at 320, 390, and 1440 pixels verify palette tokens, green root/body canvas, paper surface without exposed green bands, selection color, and no page overflow or runtime exceptions. Screenshots were inspected. Existing dark modes also pass. The news reader includes narrow-screen wrapping for article controls/text found during this review; hiring CTA text retains sufficient contrast on red.

Local build/browser evidence is retained outside this repo in the rollout directory. Production status and screenshots are recorded after release; this local QA result does not assert production has already changed.
