---
type: topic
---
## Overview


## Open questions
- 

## Linked to this topic
```base
filters:
  and:
    - file.hasLink(this.file)
    - '!file.inFolder("80 Templates")'
views:
  - type: table
    name: Ideas
    filters:
      and:
        - 'type == "idea"'
    order:
      - file.name
      - file.mtime
  - type: table
    name: Sources
    filters:
      and:
        - file.hasProperty("zotero-key")
    order:
      - file.name
      - title
      - creators
      - year
```
