# Special Repository

This is a special GitHub repository which act as a fallback for all repositories that don't have an actual `.github` directory with issue templates and other community health files. It can be also used to manage starter workflows.

## Starter workflows

Starter workflows allow everyone in the organization who has permission to create workflows to do so more quickly and easily. When you create a new workflow, you can choose a starter workflow and some or all of the work of writing the workflow will be done for you. You can use starter workflows as a starting place to build your custom workflow or use them as-is.

All starter workflows defined in this repository appear when you click on button `New workflow` from `Actions` menu.

### Workflows repository layout

Starter workflows have to be located in `workflow-templates` directory and you have to create 2 files:

* a YAML file which contains the workflow (e.g.: `my-template.yml` )
* a JSON file which contains the metadata of your workflow (e.g.: `my-template.properties.json`)

:warning: **IMPORTANT**: The metadata file must match the name of workflow file and must finish with `.properties.json`

### Naming convention

As all the workflows and their associated metadata file have to be located into the same directory, we have to setup a naming convention to stay organized. The name of the workflow should be clear, lower cases alphanumeric characters with hyphens to separate compound names. We can add a suffix to determine the usage of the workflow.

Example of suffixes:

* ci (continuous integration) ==> docker-**ci**
* pr (pull request) ==> docker-**pr**
