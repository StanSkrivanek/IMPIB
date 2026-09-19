# IMPIB public changelog

These are approved, user-facing release notes. Internal plans and unreleased work remain in the private application repository.

## 0.9.1 — 2026-09-19

- Makes JXL availability consistent across Standard, Advanced, and comparison previews, while keeping upload and codec memory limits distinct and centrally enforced.
- Prevents standalone optimization from overlapping image-set generation and invalidating in-flight template results.
- Keeps the optimized state intact when the focal-point editor remounts the Advanced inspector; only a new source image resets it.
- Adds regression tests for JXL safety decisions, format selection, and optimization state transitions.
