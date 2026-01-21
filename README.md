#Repo branch documentation

This project uses several git branches to develop and use new features into the number guessing game.
descripption of the branch structure based on the repository history seen:

## Initial State

- main 
this is the original production branch.
It contains the initial working version of the number guessing game, created in commit 45767c4.

## Dev Branch 
- dev
the dev branch serves as the master integration branch for new features 
it contains general improvements such as an encouraging message for players, created in commit 5f95961.
all completed feature branches are eventually merged into dev before going to main.

## Feature Branches
 
### feature 1
This branch added several user experience improvements such as" - 
- ability to quit the game through negative number
- play again loop 
- better feedback messages for guessing 
- additional documentation in the code 

the commits n this branch show incremental developmental steps that later merge into dev.

### feature 2 
This branch focused on adding game control logic:
- maximum number of attempts constant 
- game-over condition when attempts are exceeded 
- logic to properly stop the game after too many guesses 

it containts two main commits that implement these features 

### feature 3 
this branch represents experimental development with multiple commits:
- started hint
- got it done 
- had to fix 
- done 

these commits show messy development process and will be squashed intoa  single commit before merging 

## Hotfix Branch 

- hotfix 
this branch contains an urgent fix to the random number generation logic
corrects a bug that affected gameplay 
the fix is intended to be cherry-picked directly into main and later merged into devv

## Summary

The repository demonstrates a common Git workflow:

- main holds stable releases
- dev integrates completed features
- feature branches are used for isolated development 
- hotfix branches handle urgent fixes 

This structure allows multiple features to be developed in parallel while keeping the main branch stable.

## Learning Summary

### Merge vs Rebase
- **Merge**: Creates a merge commit, preserves branch history (feature1, feature3)
- **Rebase**: Rewrites history, creates linear timeline (feature2)
- **Squash**: Combines multiple commits into one (feature3 hint commits)
- **Cherry-pick**: Applies specific commits to different branches (hotfix to main)

### Observations
- **feature1**: Used merge - preserved history but created extra merge commits
- **feature2**: Used rebase - linear history but lost original branch context  
- **feature3**: Squashed before merge - clean history with single meaningful commit
- **hotfix**: Cherry-picked to main - applied critical fix without merging entire branch

### When to Use Each
- **Merge**: When collaborating with others, want to preserve history
- **Rebase**: Solo feature branches, want clean linear history
- **Squash**: Before merging to main/dev to clean up WIP commits
- **Cherry-pick**: Critical fixes that need to go to multiple branches

## Learning Summary

Completed Task 2 steps: feature merges, rebasing, squashing, cherry-picking.
Gained experience with Git workflows and conflict resolution.

## GitHub Workflow Practice
- Created PRs on GitHub
- Practiced code review workflow
