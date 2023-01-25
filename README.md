# tableau_cicd

# Secrets

To setup the workflows you need to define the following secrets in github actions:

| Secret Name        | Description (ignore quotes for the example values)                                      |
| ------------------ | --------------------------------------------------------------------------------------- |
| TABLEAU_URL        | The URL of your tableau server like "https://prod-useast-a.online.tableau.com"          |
| SITE               | Your site name. EX: "githubactions"                                                     |
| USERNAME           | Your username                                                                           |
| PASSWORD           | Your password                                                                           |


# Parameters

Now its possible to create project files on the directory "projects". The file will be used when you create a new PR.

```yml
WORKBOOK_NAME: Superstore
WORKBOOK_FILE: Superstore.twb
PRODUCTION_PROJECT: Superstore
STAGING_PROJECT: Superstore_Staging_1
```

Each file needs the following attributes:

| Attribute Name     | Description (ignore quotes for the example values)                                      |
| ------------------ | --------------------------------------------------------------------------------------- |
| WORKBOOK_NAME      | The workbook name. EX: "Superstore"                                                     |
| WORKBOOK_FILE      | The workbook filename with relative path. EX: "Superstore.twb" or "workbooks/Test.twbx" |
| PRODUCTION_PROJECT | Project name for PRODUCTION                                                             |
| STAGING_PROJECT    | Project name for STAGING                                                                |


Note: Please, create a new file per project. The name of the file doesn't matter, but the file needs to be a "yml" file.

:)
