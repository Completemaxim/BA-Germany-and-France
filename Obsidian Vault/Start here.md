# Start here

## Folders
| Folder | What goes in it |
|---|---|
| **00 Inbox** | Quick ideas and anything unsorted. Clear it out once a week. |
| **10 Projects** | Thesis, seminar papers: anything with a deadline. One folder per project, with a dashboard note of the same name. |
| **20 Courses** | One folder per course: a course note plus lecture notes. |
| **30 Notes** | *Ideas* (one idea per note, the title is a full sentence) and *Topics* (broad themes). |
| **40 Sources** | ZotFlow's source notes. ZotFlow creates these; don't add notes here yourself. |
| **50 Bases** | Overview tables: sources, ideas & topics, courses. |
| **60 Journal** | Optional daily research log. |
| **80 Templates** | Templates. |
| **90 Archive** | Finished projects and courses. |
| **Attachments** | Images and files. |

## One-time setup
1. **Settings → Core plugins:** turn on *Templates*, *Daily notes* and *Bases*.
2. **Settings → Templates:** set *Template folder location* to `80 Templates`.
3. **Settings → Daily notes:** set *New file location* to `60 Journal` and *Template file location* to `80 Templates/Daily note`.
4. **Settings → Files and links:** set *Default location for new attachments* to *In the folder specified below*, then choose `Attachments`.
5. **Settings → Community plugins:** install and enable **ZotFlow** and **Kanban**.
6. **Settings → ZotFlow → Source Notes:**
   - *Template Path*: `80 Templates/ZotFlow source note.md`
   - *Library Source Note Path Template* and *Local Source Note Path Template*: make them start with `40 Sources/` instead of `Source/`.
   - Then press Ctrl/Cmd+P and run **ZotFlow: Force update all library source notes**.
7. Right-click **Home** and choose **Bookmark** so you can always get back to it.

## Everyday use
- **Source:** read and highlight in ZotFlow. For your own notes on it, open the source note and run **ZotFlow: Create child note for current source note** (Ctrl/Cmd+P). The note appears under **Notes** and syncs with Zotero. In its properties, set `status` and add the project, for example `BA Thesis`, to `projects`.
- **Idea:** create a new note in `30 Notes/Ideas` and insert the *Idea* template (Ctrl/Cmd+P → *Templates: Insert template*). Add the project to `projects`.
- **Topic:** create a new note in `30 Notes/Topics` with the *Topic* template. It automatically lists every idea and source that links to it.
- **Course:** create a folder in `20 Courses`, then a note with the *Course* template. For lectures, use the *Lecture* template and set `course` to a link to the course note. They then appear on the course page.
- **Supervisor meeting:** in the project's `Meetings` folder, create a note named like `2026-10-15 Supervisor` and insert the *Meeting* template.
- **New project** (seminar paper, MA thesis): create a folder in `10 Projects` with `Chapters` and `Meetings` subfolders. Add a note with the same name as the folder and insert the *Project* template. Use that name in `projects`.
- **Finished?** Move the project or course folder to `90 Archive`.

## Property values
- **Sources, `read`:** checkbox, tick it when you have read the source. `status` (optional): to-read · reading · read · used
- **Chapters, `status`:** outline · drafting · revising · done
- **Projects and courses, `status`:** active · done
- **Source type:** Zotero tags `type/academic`, `type/grey`, `type/newspaper`, `type/comment`, or the `sourceType` property in Obsidian

> [!warning] Don't insert *ZotFlow source note* as a template yourself. ZotFlow uses it automatically.
