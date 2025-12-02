# Remote Repository Setup

## Current Remotes

\[Вставьте вывод git remote -v]
backup  git@github.com:ailovenick/techstart-api-backup.git (fetch)

backup  git@github.com:ailovenick/techstart-api-backup.git (push)

origin  git@github.com:ailovenick/techstart-api.git (fetch)

origin  git@github.com:ailovenick/techstart-api-backup.git (push)

origin  git@github.com:ailovenick/techstart-api.git (push)



## Tracking Branches

\[Вставьте вывод git branch -vv]
develop ee3707b \[backup/develop: gone] change api.py 1.1.0-dev

\* main    fb63e45 Merge branch 'main' of github.com:ailovenick/techstart-api



## Fork Workflow Summary

* Original repository: https://github.com/ailovenick/awesome-calculator
* Fork repository: https://github.com/ailovenick/calculator-fork
* Upstream configuration: git remote add upstream https://github.com/ailovenick/awesome-calculator

## Backup Strategy

* Primary remote: origin https://github.com/ailovenick/techstart-api
* Backup remote: backup https://github.com/ailovenick/techstart-api-backup
* Sync command: git remote set-url --add --push origin https://github.com/ailovenick/techstart-api-backup

Lessons Learned 
Гит гибкая система для паралельных разработок и взаимосвязи с множеством remote, можно рабоать сразу с несколькими репозиториями, развивать свою ветку какого-то уже готового проекта и одновременно подтягивать/сливать актуальные обновления. Даже есть вариант создания отдельного ремоута all и привязать к нему все url, чтобы не мешать origin, backup и тд.

