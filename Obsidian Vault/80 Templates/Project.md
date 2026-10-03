---
type: project
status: active
deadline: 
---
## Research question
> 

## Outline
- 

## Tasks
- [ ] 

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
