On GitHub:
1. Modify README.md, commit

Locally:
1. Create a branch (`git switch -c update3`)
2. Modify README.md 
3. Add a new file
4. Stage changes, commit (`git commit -a -m "changes for github"`)
6. Push (`git push origin update3`)

On GitHub:
1. Create a pull request
2. Notice we can't automatically merge it

Locally:
1. Switch to main (`git switch main`)
2. Pull changes (`git pull`)
3. Switch to branch (`git switch update3`)
4. Merge changes into branch (`git merge main`)
5. Resolve merge conflicts
6. Push branch (`git push origin update3`)

On GitHub:
1. Go back to pull request, note that it is mergeable
2. Inspect diff
3. Merge the PR

Locally
1. Switch to main (`git switch main`)
2. Pull (`git pull`)
3. Inpsect log (`git log`)
