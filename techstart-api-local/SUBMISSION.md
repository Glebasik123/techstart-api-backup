# Remote Repositories Assignment

## Repository Links

### Open Source Contribution
- Original repository: https://github.com/Glebasik123/techstart-api
- Fork repository: https://github.com/Glebasik123/calculator-fork (форк)
- Feature branch: feature/multiply

### Corporate Project  
- Main repository: https://github.com/Glebasik123/techstart-api
- Backup repository: https://github.com/Glebasik123/techstart-api-backup

## Verification Commands

Run these commands in techstart-api-local:
```
git remote -v | grep -c "push"
git branch -r | wc -l
```

Expected output: 
- First command: 4 or more (multiple push URLs)
- Second command: number of remote branches
