---
type: project
status: active
deadline: 
---
## Research question
> 

## Outline
1. [[BA 1 – Introduction]]
2. [[BA 2 – State of research]]
3. [[BA 3 – Theory & method]]
4. [[BA 4 – Analysis]]
5. [[BA 5 – Discussion]]
6. [[BA 6 – Conclusion]]

## Tasks
[[BA Thesis – Tasks|Open the task board]]

## Supervisor
- **Name:** 
- **Meeting notes:** create them in the `Meetings` folder with the *Meeting* template

## Chapters
```base
filters:
  and:
    - file.inFolder(this.file.folder + "/Chapters")
views:
  - type: table
    name: Chapters
    order:
      - file.name
      - status
    sort:
      - property: file.name
        direction: ASC
```

## Sources
```base
filters:
  and:
    - file.hasProperty("zotero-key")
    - projects.toString().contains(this.file.name)
views:
  - type: table
    name: Sources
    groupBy:
      property: status
      direction: ASC
    order:
      - file.name
      - title
      - creators
      - year
```

## My ideas
```base
filters:
  and:
    - 'type == "idea"'
    - projects.toString().contains(this.file.name)
views:
  - type: table
    name: Ideas
    order:
      - file.name
      - file.mtime
```

## Meetings
```base
filters:
  and:
    - file.inFolder(this.file.folder + "/Meetings")
views:
  - type: table
    name: Meetings
    order:
      - file.name
      - date
    sort:
      - property: date
        direction: DESC
```
