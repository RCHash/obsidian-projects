---
type: person
projects: 
email: 
status: 
---
#Resource

# 1. Meetings:
>[!info]- ## 1.1. Attended:
>```dataview
>TABLE project_code AS Project, date(date) AS Date
>WHERE contains(attendees,this.file.link) AND type="meeting"
>```

>[!info]- ## 1.1. Unattended:
>```dataview
>TABLE project_code AS Project, date(date) AS Date
>WHERE contains(cc,this.file.link) AND type="meeting"
>```

# 2. Tasks:
>[!info]- ## 2.1. TODO:
>```dataview
>TASK
>WHERE contains(assigned,this.file.link)
>GROUP BY project_code
>```

>[!info]- ## 2.2. DONE:
>```dataview
>TASK
>WHERE contains(assigned,this.file.link)
>GROUP BY project_code
>```
