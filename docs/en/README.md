Rename the default branch from your Git repository both on server and local.

# Instructions

1. Check for all dependencies that could break if the default branch name is changed, such as CI/CD pipelines, internal and external integrations, automations, documentations. To help when it is really changed try to:

    - Change in advance the usage of the branch name to a variable.
    - Write down all you need to do after the renaming.
    - Communicate everyone what is being renamed and when.

2. Rename the default branch on your Git remote server.

    - [GitHub](GitHub.md)
    - [GitLab](GitLab.md)

3. Run this script on the directory of each clone of the repository. Tell others to do the same.

        curl -fsSL https://raw.githubusercontent.com/ResultadosDigitais/rename_default_branch/main/rename_default_branch | bash

# Configuration

If you are not renaming from `master` to `main`, set the desired values:

    curl -fsSL https://raw.githubusercontent.com/ResultadosDigitais/rename_default_branch/main/rename_default_branch | FROM=old-branch TO=new-branch bash

Options:

- `REMOTE`: Git remote name
- `FROM`: Current default branch name
- `TO`: New default branch name
