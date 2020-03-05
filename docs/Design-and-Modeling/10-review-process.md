# Design Review Process

When you're a solo developer working on an API design, the process is pretty simple:

1. Make some changes
2. They're great
3. Ship it

When multiple developers are working on the API, and when multipe teams are all making multiple APIs, quality control can suddenly feel a bit more important. 

Most developers are used to changing to source code in version control systems via "pull requests", at which point various teammates or other folks will review the code. Seeing as Stoplight lets you continue to use your git repo as a source of truth for your API descriptions, this same process can be used for OpenAPI and JSON Schema reviews too!

## 1. Open a Project in Studio

[Create or open a Project](../Basics/01-working-with-projects.md) in Studio Web or Desktop.

## 2. Create a new Branch

A lot of Git repositories (especially those on GitHub) are configured to use [protected branches](https://help.github.com/en/github/administering-a-repository/about-protected-branches), which means pushing to master is not possible. Maybe you can push to master, maybe not, but if you'd like other people to review your work, it is best to create a branch to keep the changes out of master until they've been reviewed.

![At the bottom left of Stoplight Studio there is a small panel which shows the name of the current branch. This may be master if you've never changed it. Click that to see how to switch branches.](../../assets/images/switch-branch.png)

A drawer will appear in the middle of the screen, allowing you to search through existing branches. To make a new one, type in a name for a branch which does not exist. If you are adding a new endpoint, the branch could be `new-companies-endpoint`. 

![Typing a new branch name into the drawer in Studio.](../../assets/images/create-branch.png)

Hit enter or click the "(+)" icon and you've switched (a.k.a "checked out") the new branch.

## 3. Make Changes, Commit, & Push

When you're done making changes, [commit them, then push](./09-working-with-projects.md) send the branch up to the repository.

## 4. Publish Branch on Stoplight

There are a few ways to Publish documentation:

- [Manually via Studio](../Documentation/06-publishing.md)
- [Automatically via Continuos Integration](../Documentation/07-publish-via-ci.md)
- _**Coming Soon:** Git webhooks for autopublish!_

## 5. Open a Pull Request

How you create a pull request depends on where the project's repository is hosted:

- **BitBucket:** [Create a Pull Request](https://www.atlassian.com/git/tutorials/making-a-pull-request)
- **Gitea:** [Create a Pull Request](https://docs.gitea.io/en-us/pull-request/)
- **GitHub:** [Create a Pull Request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)
- **GitLab:** [Create a Merge Request](https://docs.gitlab.com/ee/user/project/merge_requests/)

## 6. Link to Branch Documentation

Once you

## Future Simplifications

There are plans to refine this process, to make people not need to flip between Studio and the version control system interface. For example, soon you will be able to create pull requests right from the Studio interface, publishing will happen automatically via webhooks, and Stoplight will automatically add links to the branches documentation on the pull request, to save people manually doing that bit.

This all means Design Reviews will become more accessible for non-technical people, and a litle less combersome for technical people. For now though, at least the process is very familiar for developers, and follows the standard pull-request flow for your VCS of choice.
