---
title: Thesaurus MOC
type: moc
---

# Terminology

```dataview
TABLE definition_ru AS "Definition", source_author AS "Author", tags AS "Tags"
FROM "Business/Thesaurus"
WHERE type = "term"
SORT file.name ASC
```
