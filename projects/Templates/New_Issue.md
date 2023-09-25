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

>[!info]- # 1. Description:
>description::

>[!info]- # 2. Related Meetings:
>```dataview
>TABLE date AS Date
>FROM !"Templates"
>WHERE contains(related_issues,this.issue_code) AND type="meeting"
>```
