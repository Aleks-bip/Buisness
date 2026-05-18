---
title: Formulas MOC
type: moc
---

# Formulas & Patterns

```dataview
TABLE
  quote_en AS "Quote",
  source_author AS "Author",
  theme AS "Theme"
FROM "Business/Formulas"
WHERE type = "formula"
SORT date_processed DESC
```
