# dino-park-insomnia

Sandbox/experiment repository to try out [Insomnia](https://insomnia.rest)'s Git Sync features. This Insomnia collection is configured to run APIOps with Azure DevOps + Azure pipelines

## Prerequisites

- [DecK](https://github.com/Kong/deck) (for Kong Configuration management)
- [Insomnia](https://github.com/Kong/insomnia/releases) (use version `2022.3.0-beta.4` and up)
- Kong Gateway installed
- [Azure Pipeline agent running](https://learn.microsoft.com/en-us/azure/devops/pipelines/agents/linux-agent?view=azure-devops) (self-hosted agents are used in this case)

## Run
This repo is meant for running APIOps on Azure environment. Hence the instructions are based on importation from Azure DevOps environment. Clone this repo to an Azure DevOps Repo if necessary. 

- Import this repository on Insomnia via Git (link to repo is: `https://github.com/raylaijh/apiops-demo-azure.git`)
- Perform a change on Insomnia and commit to Azure DevOps repo. Pipeline should trigger CICD flow for APIOps. Review azure-pipelines.yml for details of each CICD steps defined in this flow.

## Other

