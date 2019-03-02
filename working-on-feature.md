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

a