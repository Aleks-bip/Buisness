---
title: Business Knowledge Base
type: moc
---

# Business Knowledge Base

## Corpus (Sources)

```dataview
TABLE source_author AS "Author", source_type AS "Type", date_processed AS "Processed", themes AS "Themes"
FROM "Business/Nate Corpus"
WHERE source_author != null
SORT date_processed DESC
```

## Frameworks

```dataview
TABLE description AS "Description", source_author AS "Author"
FROM "Business/Frameworks"
WHERE type = "framework"
SORT file.name ASC
```

## Terminology

```dataview
TABLE definition_ru AS "Definition", tags AS "Tags"
FROM "Business/Thesaurus"
WHERE type = "term"
SORT file.name ASC
```

## Formulas

```dataview
TABLE quote_en AS "Quote", source_author AS "Author"
FROM "Business/Formulas"
WHERE type = "formula"
SORT date_processed DESC
```
