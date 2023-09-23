---
type: project
project_code: Project_2
name: Another Project
active: yes
governance: waterfall
phase: conceptual
coordinator: john_doe
client: internal_client
sponsor: internal_sponsor
---
TAGS:: #Project

# 1. Business Case:
>[!info]- ## 1.1. Purpose:
>

>[!info]- ## Expected Gains:
>

# 2. Team:
>[!info]- ## 2.1. Team Members:
>```dataview
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
>```

>[!info]- ## 4.2. Closed:
>```dataview
>```

# 5. Tasks:
>[!info]- ## 5.1. Overview:
>```dataview
>```

>[!info]- ## 5.2. To-Do:
>```dataview
>```

>[!info]- ## 5.3. Done: