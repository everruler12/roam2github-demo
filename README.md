## roam2github-demo

# This is now out of date! Use [roam2github-actions](https://github.com/everruler12/roam2github-actions)

---

### [Click here for the full guide](https://www.notion.so/Roam2Github-Backup-Guide-650925859a4a42cf940e3fb74f5189f9)

## Update instructions for Roam-to-git users who followed my [old guide](https://eriknewhard.com/blog/backup-roam-in-github):

For those who are having issues with [MatthieuBizien/roam-to-git](https://github.com/MatthieuBizien/roam-to-git/) in GitHub Actions, try my new solution:

1. Add secrets for the following values:

    - `ROAM_EMAIL`
    - `ROAM_PASSWORD`
    - `ROAM_GRAPH`
        - Now with multi graph support! Just add graph names on separate lines in `R2G_GRAPH`. (Or separate them by commas.)
    
2. Update your main.yml with the code here: https://github.com/everruler12/roam2github-actions/blob/main/.github/workflows/main.yml

This will backup Markdown, JSON, and EDN!

Check here for additional [main.yml settings](https://github.com/everruler12/roam2github/blob/main/documentation/Settings%20for%20main.yml.md)
