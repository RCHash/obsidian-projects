---
type: issue
issue_code: 
subtype: change request, problem, concern, off-specification, good idea
project_code: 
status: open
raised_date: {{date}}
priority: 
severity: 
closure_date: 
---
raised_by:: 
solver:: 

>[!info]- # 1. Description:
>description::
>budget_impact:: 
>related_issues:: 

>[!info]- # 2. Related Meetings:
>```dataview
>TABLE date AS Date
>FROM !"Templates"
>WHERE contains(related_issues,this.issue_code) AND type="meeting"
>```

>[!info]- # 3. Related Pending Tasks:
>```dataview
>TASK
>FROM !"Templates"
>WHERE contains(related_issues,this.issue_code) AND !completed
>```
