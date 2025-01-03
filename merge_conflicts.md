(Draw commits & branches on board as we go)

# Simple merge conflict

1. Create branch (`git switch -c update1`)
2. Modify README.md, stage, commit (`git commit -a -m "Change readme update1"`)
3. Checkout main, create new branch (`git switch main`, `git switch -c update2`)
4. Show branches (`git branch`)
5. Modify README.md, stage, commit (`git commit -a -m "Change readme update2"`)
6. Checkout main (`git switch main`)
7. Merge update 1 (`git merge update1`)
8. Try to merge update 2, get merge conflict (`git merge update2`)
9. Resolve conflicts and merge

# Resolve conflicts on branch instead of at merge time

1. Reset main to abandon second merge (`git reset HEAD^`)
2. Inspect log (`git log`)
3. Checkout update2 (`git switch update2`)
4. Merge main->update2 (`git merge main`)
5. Inpsect log (`git log`)
6. Switch to main (`git switch main`)
7. Merge update2->main (`git merge update2`) - note "fast forward"
