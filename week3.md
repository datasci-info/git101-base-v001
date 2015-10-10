# Week3

## 前情提要

## 分散式版控—— Forking Workflow

## Forking vs. Branch

## Forking Workflow SOP

## Multiple remote

### Bitbucket

## Advanced rebase (rollback)

- `git rebase -i`

## 合併repo (應該講解就好，最後使用）

- `git remote add $Remote_Name $GIT_URL`
- `git fetch $Remote_Name`
- `git subtree add -P $New_Local_DIR $Remote_Name/$Branch `

## 不小心commit敏感資料該如何處理

- [永久刪除 資料夾] 
  - `git filter-branch --force --index-filter 'git rm -r --cached --ignore-unmatch $DIR_PATH' --prune-empty --tag-name-filter cat -- --all`
- [永久刪除 檔案] 
  - `git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch $FILE_PATH' --prune-empty --tag-name-filter cat -- --all`
- [保留 資料夾 / 其他永久刪除] 
  - `git filter-branch -f --prune-empty --subdirectory-filter $DIR_PATH --tag-name-filter cat -- --all`

## gitbook

### gitbook 連結 github

## 總攻擊前的叮嚀（總複習）

## 魔王關～～36人大亂鬥
