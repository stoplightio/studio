# Git Credentials

Studio Web will use the Git Credentials associated with your Stoplight account depending on the Git provider being used. That means if you connect a GitHub and a BitBucket account, and work on a Git Project which is hosted on BitBucket, it's going to know to use the BitBucket credentials. You don't need to think about it at all.

Studio Desktop v1.x used to ask you to log in to your Stoplight account in order to use Git functionality for things like commits, pushing, pulling, etc. but you no longer need to bother with that. You can work with any VCS provider by adding your Git credentials for that provider.

You should be asked to add credentials for a provider the first time you add that project, but if for some reason that doesn't work, or you need to change them, here's how it works.

## Adding Credentials for Github

1. Create a [new personal access token](https://github.com/settings/tokens/new) (more information in the [creating personal access tokens guide on Github](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).

2. Choose "repo" permissions to allow enable read/writing files in your Git repository then generate the token.

![image](../assets/images/git-creds-github-token.png)

3. Click the Cog icon bottom left to open Project Settings, click Project Settings, and click the "+ Credential" button.

- **Host URL:** `https://github.com/`
- **Username:** Your GitHub username, e.g.: `janesmith123`
- **Password:** The Personal Access Token you just created
- **Author Name:** A display name, usually a full name, e.g.: `Jane Smith`
- **Author Email:** Your GitHub email address

Job done! You should now be able to push to GitHub.

> Keep in mind that these credentials are stored on your local computer as a security measure, so if you switch computers you'll need to repeat this step.

## Other Git Providers

The instructions are pretty similar for all the other Git providers we support: GitLab, BitBucket Cloud, BitBucket Server, Gitea, Azure, etc. Generally you want to point your Host URL to the main host of the server, so for GitLab that'll be `https://gitlab.com/` 

If they support personal access tokens you can use that instead of entering your actual password, but not every provider supports this.

## Working with Git

Once this is done, check out our guide on [Common Git Tasks](Basics/04-common-git-tasks.md) to get pushing, pulling, switching branches and all sorts of other Git magic.
