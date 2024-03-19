Disable cors

```bash
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --disable-web-security --disable-gpu --user-data-dir=~/chromeTemp
```
or
```bash
"C:\Program Files\Google\Chrome\Application\chrome.exe" --disable-web-security --disable-gpu --user-data-dir=~/chromeTemp
```


Revert Last commit not pushed
```bash
git reset HEAD~1
```

Revert Last pushed commit
```bash
git reset --soft HEAD^1
git commit -m "commit name"
git push -f
```

Change branch name local and remote
```bash
 1. git checkout <old_name>
 2. git branch -m <new_name>
 3. git push origin -u <new_name>
 4. git push origin --delete <old_name>
```

Remove commits from remote
```bash
 1. git rebase -i HEAD~1
 2. Above you should see (pick <commit hash> ) . Remove this line
 3. git push origin +branchName
```


Git push with access token
```bash
git push https://<GITHUB_ACCESS_TOKEN>@github.com/<GITHUB_USERNAME>/<REPOSITORY_NAME>.git
```

Save git credentials
```bash
git config --global credential.helper store
```
