## roam2github-demo

# Don't fork this demo repo for your backups!

The demo backups will be included, and your backups will be public. You should create your own **private** repo and copy the code from main.yml.

### [Click here for the main README with full instructions and explanations](https://github.com/everruler12/roam2github)

## Update instructions for Roam-to-git users who followed my [old guide](https://eriknewhard.com/blog/backup-roam-in-github):

For those who are having issues with [MatthieuBizien/roam-to-git](https://github.com/MatthieuBizien/roam-to-git/) in GitHub Actions, try my new solution:

1. Add secrets for the following values:

    - `R2G_EMAIL`
    - `R2G_PASSWORD`
    - `R2G_GRAPH`
        - Now with multi graph support! Just add graph names on separate lines in `R2G_GRAPH`. (Or separate them by commas.)
    
2. Update your main.yml with the code here: https://github.com/everruler12/roam2github-demo/blob/main/.github/workflows/main.yml

    - _If you created your repo before October 1st, 2020, you may need to change the branch name from 'main' to 'master'_

This will backup Markdown, JSON, and EDN!
