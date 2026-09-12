# Architecture Overview

DocDiffGUI is organized around a PDF comparison engine and a desktop GUI.

```text
┌───────────────────────────┐
│        Desktop GUI        │
│          PyQt5            │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│     Comparison Engine     │
│       compare_pdfs()      │
└─────────────┬─────────────┘
              │
       ┌──────┴──────┐
       ▼             ▼
   PDF 1           PDF 2
       │             │
       └──────┬──────┘
              ▼
      Difference Analysis
              │
              ▼
       Report Generation
              │
              ▼
      PDF / Review Output
```

The implementation supports configurable comparison behavior, page pairing/ranges, multiple comparison modes, and report generation.

This document is intentionally high-level. Keep proprietary production architecture and licensing infrastructure private.
