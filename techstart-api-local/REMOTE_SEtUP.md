# Remote Repository Setup

## Current Remotes
backup git@github.com:Glebasik123/techstart-api-backup.git (fetch)
backup git@github.com:Glebasik123/techstart-api-backup.git (push)
origin git@github.com:Glebasik123/techstart-api.git (fetch)
origin git@github.com:Glebasik123/techstart-api.git (push)
origin git@github.com:Glebasik123/techstart-api-backup.git (push)

## Tracking Branches
main [origin/main] Merge remote changes with local changes
develop [origin/develop] Change version to 1.1.0-dev


## Fork Workflow Summary
- Original repository: git@github.com:Glebasik123/awesome-calculator.git
- Fork repository: git@github.com:Glebasik123/calculator-fork.git  
- Upstream configuration: `git remote add upstream git@github.com:Glebasik123/awesome-calculator.git`

## Backup Strategy
- Primary remote: origin (techstart-api)
- Backup remote: backup (techstart-api-backup)
- Sync command: `git remote set-url --add --push origin git@github.com:Glebasik123/techstart-api-backup.git`

## Lessons Learned
1. Всегда делать `git fetch` перед работой с ветками чтобы получить актуальную информацию с remote
2. Настраивать upstream для форков чтобы легко синхронизироваться с оригинальным репозиторием
3. Использовать `git remote -v` и `git branch -vv` для проверки текущей конфигурации
4. Решать конфликты через `git pull` с merge стратегией для сохранения истории изменений
