# Forge Pull Requests

Create a pull request on GitHub or GitLab within the comfort of Spacemacs, using all the usual editor tools to write pull request descriptions.

Magit Forge will use a Pull Request template if one is added to the repository.


## Create a pull request

Assumes you have a fork and original repository as remotes added to the local git repository.

Create a branch on the fork with a descriptive name of the change you want to submit as a pull request.  Commit changes to that new branch.

`P p` to push the change to the remote repository for the fork.

`@` to open the forge menu from the Magit Status buffer.

`r` to select the repository that the pull request will be created on (eg. the upstream repository, not the fork).

![Spacemacs Magit Forge - create pull request forge repository](/images/spacemacs-magit-forge-create-pull-request-forge-repository.png)

`c p` to create a new pull request.

For the source repository, select the branch of the local fork repository.

![Spacemacs Magit Forge - create pull request source branch](/images/spacemacs-magit-forge-create-pull-request-source-branch.png)

For the target repository, select the upstream repository

![Spacemacs Magit Forge - create pull request target branch](/images/spacemacs-magit-forge-create-pull-request-target-branch.png)

The description of the change is show and can be edited for the pull request description.

`, ,` to confirm the message and create the pull request on the upstream repository. `, k` to cancel the pull request.

![Spacemacs Magit Forge - create pull request text](/images/spacemacs-magit-forge-create-pull-request-text.png)


## Create a draft pull request

A pull request can be marked as a draft when created by Magit Forge, to communicate that the PR is not ready for review or approval.

With the pull request buffer opened, add yaml style front matter to the to define the PR as a draft.

```yaml
---
draft: true
---
```


## Example pull request

An example of using Emacs to create a pull request, with a pull request template from the repository.

A template can be quickly edited using all the Emacs tools you are used to having.

![Spacemacs Magit Forge - example of creating a pull request with template](https://raw.githubusercontent.com/practicalli/graphic-design/live/spacemacs/screenshots/spacemacs-magit-forge-pull-request-edit.png)
