# devops-intro-2024

A test repo intended for Salesforce graduates.

# Task

1. Perform the `First-time Install` (see below)
1. Do `Clone Repo` (see below)
1. Gain access to Trello ([accept invite](https://trello.com/invite/66ba1506225bb2355eb282bc/ATTIabf86382ad515ec97d9ca4050cdf281aD4F33765))
1. Open the [Trello Board](https://trello.com/b/3zdLyE5R/devops-intro-2024)
1. Start by picking items from the Backlog
1. Follow the `Make Changes` guide below to make changes

# First-time Install

Make sure you've performed the steps in [Local Setup](docs/devops/local-setup.md) before trying to create a Scratch Org.

# Clone Repo

1. Open the repo in your browser
1. Click `Code` → `Open with GitHub Desktop`
1. Save the repo somewhere on your computer
    - _**Avoid cloud-synced folders!**_
    - On Windows, the `Documents` folder is synced to OneDrive and will cause issues later!
1. In GitHub Desktop, click `Repository` → `Open in X`
    - Depending on your system you can have X = `Command Line`, `Git Bash` og `Terminal`
    - Once opened, type and run `npm install`
    - This will install all necessary software for you, including code formatting.

# Make Changes

1. In GitHub Desktop, click `Repository` → `Open in X`
    - Depending on your system you can have X = `Command Line`, `Git Bash` og `Terminal`
1. Run `npm run scratch:create`
    - Now, a fully functioning copy of production (without data) will be created for you.
1. Make your changes inside the Scratch Org
1. Run `npm run scratch:pull` to add the changes from the Scratch Org to your local computer
1. Commit & Push the changes inside GitHub Desktop
1. Create a Pull Request
    - To `main` or `preprod`, depending on use case
    - Get the changes validated successfully
    - If Slack Integration is working, a post is added for others to code review your changes. Otherwhise, get someone to approve it.
1. Merge the PR
1. Check the package creation status in the `Actions` tab
1. Once the package is done, check it in the `Code` tab → `Releases`
1. Click `Deploy` on the release you want to deploy to production
    - Click `Run Workflow`
    - Keep `Branch: main` if you want to deploy the latest package.
    - If you want a specific package, click the dropdown → `Tags` → Choose the version
    - Finally, click `Run workflow` again to deploy
    - Wait a couple of seconds, and a new entry should appear in the list. You can open it to view the progress of the deployment.
