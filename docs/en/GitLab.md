# GitLab

To rename the default branch:

1. On the sidebar go to "Repository" > "Branches".

2. Click "New branch".

3. Write the new default branch name, make sure the current default branch is selected on "Create from" and confirm.

4. On the sidebar go to "Settings" > "Repository".

5. On "Default branch" section select the new default branch and save.

6. On "Protected branches" section protect the new default branch with the name configuration used with the previous one.

That should rename the default branch but will not update merge requests targeting this branch.

You need to update each merge request to the new branch or do it with some script using the API.

Your repository will be changed only on the server, so after that continue with the guide to rename all local copies.
