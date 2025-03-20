Merge vs. Rebase

🔹 Merge	

Preserves history	

Creates a new commit	

Best for public branches	

Example of Merge:
```
git checkout main
git merge feature-branch
```

🔹 Rebase

Rewrites history

Moves commits linearly

Best for private branches

Example of Rebase:
```
git checkout feature-branch
git rebase main
```
