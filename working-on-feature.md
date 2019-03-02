#Working on new feature

## Before

- `git checkout master`
- `git pull origin master`
- `git checkout -b feature/FEATURE_ID`
  - where `FEATURE_ID` should be identifier of picked up feature, for example `backend-1`

## While working

- commit small parts of your work:  `git commit -m 'COMMIT_MESSAGE'`
  - where `COMMIT_MESSAGE` should be descriptive message rather than something like `changes`
- push to origin from time to time in case you computer explodes:
  - `git push origin feature/FEATURE_ID`

## After finishing

- `git checkout master`
- `git pull origin master`
- `git checkout -` (to return to your branch, `-` can be replaced with your branch name, e.g. `feature/backend-1`)
- `git rebase master`, in case any conflicts occur:
  - resolve them
  - `git add .`
  - `git rebase --continue`
- push all your changes to origin (`-f` option might be needed after rebasing)
- go to repository on which you've been working on (e.g. https://github.com/zagrosz/backend)
- click on `Pull requests` and `New pull request`
- select your branch on `compare` button and click `Create new pull request` and `Create pull request`

## Code review

- Every pull request needs to be reviewed by at least 2 supervisors (or 1 for one of supervisor's pull request)
- Make requested changes and/or resolve all conversations on pull request
- After getting approval from reviewers go to merging process

## Merge

-  Select `Squash and merge` option on GitHub