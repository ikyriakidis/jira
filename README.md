# jira
Useful Jira Query Language (JQL) queries

To find ALL my tickets (present + previous/historic):

```
summary ~ currentUser() OR description ~ currentUser() OR assignee = currentUser() OR assignee was currentUser() OR worklogAuthor = currentUser() OR comment ~ currentUser() OR watcher = currentUser() OR text ~ currentUser() OR creator = currentUser() OR voter = currentUser() OR Status changed by currentuser() ORDER BY updated DESC, resolved ASC
```
