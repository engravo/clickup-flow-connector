# ClickUp Flow Connector

> A swagger file to build a custom connector for Microsoft Flow to connect to ClickUp API

ClickUp API Token
---
1. Go to ClickUp and hit your face (not literally) at the bottom left
2. Klick on **Apps** and generate your API Token 

Create custom connector
---
3. Navigate to **Power Automate** (formerly Flows) > **Data** > **Custom connectors**
4. Klick on **+ New custom connector** > **Import an OpenAPI file**
5. **Enter a name** (eg. ClickUp Connector), **import the JSON-file** from the repo and hit **Continue**

General
---
6. **Upload the ClickUp logo** from the repo, **add the ClickUp brand color** (`#7b68ee`) and submit by hitting Security

Security (should be prefilled, else enter the following)
---
7. For Authentication type **choose API Key**
8. For Parameter label enter `API Key`
9. For Parameter name enter `Authorization`
10. Parameter location **choose Header**
11. Hit **Create connector** (at the topbar) and that's it.. you're ready to go.

Definitions
---
| Definition | Description |
|--|--|
| GetTeams  | Gets the teams that you are a member of |
| GetSpaces | Gets the spaces from a team team you choose |
| GetFolders | Enter a space id and get the folders that belong to that space |
| GetTaskByID | Enter a task id and get a whole lot of dynamic content you can work with in further action steps |
| GetAccessableCustomFields | Enter a list id and get all the custom fields |
| PostTaskComment | Enter a task id and post a comment |
| GetTasksFromList | Enter a list id and get all the tasks that live in there |
| CreateTask | Enter a list id and create a new task |
| ~~PostAttachment~~ | Does not work yet.. but I successfully accomplished posting attachments to a task with a workaround by using the premium HTTP connector and the POST method. Will provide more info soon. Hopefully we get that definition running which will make that workaround needless.  |

Happy flowing.. ehhh automating :)
