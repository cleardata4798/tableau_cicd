# tableau_cicd

# Secrets

To setup the workflows you need to define the following secrets in github actions:

| Secret Name   | Description (igonore quotes for the example values)                                     |
| ------------- | --------------------------------------------------------------------------------------- |
| TABLEAU_URL   | The URL of your tableau server like "https://prod-useast-a.online.tableau.com"          |
| SITE          | Your site name. EX: "githubactions"                                                     |
| USERNAME      | Your username                                                                           |
| PASSWORD      | Your password                                                                           |
| WORKBOOK_NAME | The workbook name. EX: "Superstore"                                                     |
| WORKBOOK_FILE | The workbook filename with relative path. EX: "Superstore.twb" or "workbooks/Test.twbx" |

:)
