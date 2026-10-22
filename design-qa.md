# Registry design QA

Source: approved Index / Simplified board without title marks, `08-index-simplified-no-marks.png`, pinned in littlelink PR #30.

Implementation preview: http://127.0.0.1:4350/ . Intended captures: 390x844, 768x1024, 1440x1024; deviceScaleFactor 1. Source is a multi-site board, so compare the Docs example's typography/materials with this product's real documentation, retaining all technical content rather than matching placeholder copy.

Static checks pass for all 18 HTML pages: text unchanged, every local link exists, stylesheet syntax delimiters balanced, decorative gradient and huge clamp typography removed, licensed local fonts present. Table containers are focusable named scroll regions; current navigation is identified. No application build exists.

Browser fallback permission is pending; no rendered implementation screenshot, console/interaction test, density-normalized comparison or visual pass is asserted. Required review covers fonts, spacing, colors, source-content/diagram fidelity and keyboard/reflow behavior. Capture and compare with the approved source before promoting any production domains. No P0/P1/P2 finding has been resolved by assertion.

final result: blocked
