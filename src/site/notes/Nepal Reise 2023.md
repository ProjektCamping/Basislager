```dataview
>TABLE WITHOUT ID regexreplace(Tasks.text, "\[.*$", "") AS Task, choice(Tasks.completed, "done", "todo") AS Status, Tasks.due AS "Due Date", Tasks.section AS "link" from "Nepal Reise 2023" 
>WHERE completed !=1  
>FLATTEN file.tasks AS Tasks 
>```