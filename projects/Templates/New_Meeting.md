---
type: meeting
project_code: 
medium: 
date: {{date}}
minutes: 
---
TAGS:: #Project #Meeting
attendees:: 
cc:: 

# 1. Discussion:
1. pending

# 2. Tasks:
>[!info]+
>Total Tasks: **`=(length(this.file.tasks))`**
>Done Tasks: **`=(length(filter(this.file.tasks.completed, (t) => t = true)))`**
>Cancelled Tasks: **`=(length(filter(this.file.tasks.cancelled, (t) => t = true)))`**
>`= "<progress value='" + (length(filter(this.file.tasks.completed, (t) => t = true)) / (length(this.file.tasks)-length(filter(this.file.tasks.cancelled, (t) => t = true))) * 100) + "' max='100'></progress>" + "<br>" + round(length(filter(this.file.tasks.completed, (t) => t = true)) / (length(this.file.tasks)-length(filter(this.file.tasks.cancelled, (t) => t = true))) * 100) + "% total completion"`
- [ ] task1
- [x] task2
- [ ] task3
- [-] cancelled [cancelled:: true]
