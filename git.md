# Git

## Branch
### Create Branch
`git branch *name*`
### Switch Branch
`git checkout *name*`
### Delete Branch
`git branch -d *name*`
### Rename Branch
Use: `rename_branch *old_name* *new_name*`

```bash
rename_branch() {
    git branch $2 &&
    git checkout $2 &&
    git branch -d $1
} 
```
