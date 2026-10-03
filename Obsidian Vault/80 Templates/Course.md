---
type: course
semester: 
lecturer: 
ects: 
status: active
deadline: 
---
## Overview
- **Exam / assignment:** 
- **Time & room:** 

## Lectures
```base
filters:
  and:
    - 'type == "lecture"'
    - file.hasLink(this.file)
views:
  - type: table
    name: Lectures
    order:
      - file.name
      - date
    sort:
      - property: date
        direction: ASC
```

## Readings
- 
