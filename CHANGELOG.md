# IMPIB public changelog

These are approved, user-facing release notes. Internal plans and unreleased work remain in the private application repository.

## 0.9.32 — 2026-09-20

- Keeps the Advanced Output plan unavailable until image optimization completes, with a clear prerequisite message.
- Clarifies image-set planning with Set builder and Template library tabs and a consistent summary and Generate action in both views.
- Opens Download automatically when image-set generation finishes successfully.

## 0.9.31 — 2026-09-19

- Shows responsive-width limits directly below the input, including whether upscaling is on or off.
- Clarifies that large AVIF outputs may strain browser memory and advises smaller dimensions only if optimization fails.
- Improves the visibility of large-output guidance in the light theme.

## 0.9.3 — 2026-09-19

- Improves guidance and recovery for large image and upscale jobs in the browser.
- Keeps successfully generated image-set files when AVIF cannot encode a particular size, marking that output as skipped instead of stopping the set.
- Clarifies completed image-set status when an output was skipped, while keeping valid responsive widths selectable.

## 0.9.2 — 2026-09-19

- Applies the committed crop to generated responsive images and exact-size templates, with output dimensions and framing based on the cropped source.
- Adds a browser regression test that checks the pixels in a downloaded cropped image.

## 0.9.1 — 2026-09-19

- Makes JXL availability consistent across Standard, Advanced, and comparison previews, while keeping upload and codec memory limits distinct and centrally enforced.
- Prevents standalone optimization from overlapping image-set generation and invalidating in-flight template results.
- Keeps the optimized state intact when the focal-point editor remounts the Advanced inspector; only a new source image resets it.
- Adds regression tests for JXL safety decisions, format selection, and optimization state transitions.
