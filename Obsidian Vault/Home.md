# 🎓 Home

New here? Read [[Start here]] first.

## Projects
- [[BA Thesis]] · [[BA Thesis – Tasks|Tasks]]

## Overviews
- [[Source index.base|📚 Source index]]
- [[Notes index.base|💡 Ideas & topics]]
- [[Courses.base|🏛️ Courses]]

## Upcoming deadlines
```base
filters:
  and:
    - deadline
    - 'status != "done"'
    - '!file.inFolder("80 Templates")'
views:
  - type: table
    name: Deadlines
    order:
      - file.name
      - deadline
      - status
    sort:
      - property: deadline
        direction: ASC
```

## Recently edited
```base
filters:
  and:
    - 'file.ext == "md"'
    - '!file.inFolder("80 Templates")'
    - '!file.hasProperty("zotero-key")'
views:
  - type: table
    name: Recently edited
    limit: 10
    order:
      - file.name
      - file.mtime
    sort:
      - property: file.mtime
        direction: DESC
```
