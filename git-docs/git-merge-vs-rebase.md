Merge vs. Rebase

🔹 Merge	

Preserves history	

Creates a new commit	

Best for public branches	

🔹 Rebase

Rewrites history

Moves commits linearly

Best for private branches

Example of Merge:
```
git checkout main
git merge feature-branch
```

Example of Rebase:
```
git checkout feature-branch
git rebase main
```
