---
type: meeting
project_code: 
medium: 
date: {{date}}
minutes: 
---
TAGS:: #Project 
attendees:: 
cc:: 

# 1. Discussion:
1. pending

# 2. Tasks:
>[!info]-
>Total Tasks: **`=(length(this.file.tasks))`**
>Done Tasks: **`=(length(filter(this.file.tasks.completed, (t) => t = true)))`**
>Cancelled Tasks: **`=(length(filter(this.file.tasks.cancelled, (t) => t = true)))`**
- [ ] task
- [-] cancelled [cancelled:: true]
