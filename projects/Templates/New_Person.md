---
type: person
projects: 
email: 
status: 
---
#Resource

>[!info]- # 1. Meetings:
>```dataview
>TABLE project_code AS Project, date(date) AS Date
>WHERE contains(attendees,this.name) AND type="meeting"

>[!info]- 