---
type: project
project_code: 
name: 
active: yes
governance: 
phase: 
coordinator: 
client: 
sponsor: 
---
TAGS:: #Project

# 1. Business Case:
>[!info]- ## 1.1. Purpose:
>objectives:: 

>[!info]- ## Expected Gains:
>gains::

# 2. Team:
>[!info]- ## 2.1. Team Members:
>```dataview
>TABLE disciplines AS "Discipline"
>FROM #Resource 
>WHERE type="human resource" AND contains(projects,this.project_code)
>```

# 3. Meetings:
>[!info]- ## 3.1. Overview:
>```dataview
>TABLE date(date) AS Date, medium AS Medium, minutes AS "Minutes Status"
>FROM !"Templates"
>WHERE type="meeting" AND contains(project_code,this.project_code)
>```

# 4. Issues:
>[!info]- ## 4.1. Open:
>```dataview
>TABLE severity
>FROM !"Templates"
>WHERE status="open" AND contains(project_code,this.project_code)
>```

>[!info]- ## 4.2. Closed:
>```dataview
>TABLE severity
>FROM !"Templates"
>WHERE status="closed" AND contains(project_code,this.project_code)
>```

# 5. Tasks:
>[!info]- ## 5.1. Overview:
>```dataview
>```

>[!info]- ## 5.2. TODO:
>```dataview
>TASK
>FROM #Project 
>WHERE contains(project_code,this.project_code) AND !completed AND contains(status," ")
>GROUP BY file.link
>```

>[!info]- ## 5.3. DONE:
>```dataview
>TASK
>FROM #Project 
>WHERE contains(project_code,this.project_code) AND completed AND contains(status,"x")
>GROUP BY file.link
>```
