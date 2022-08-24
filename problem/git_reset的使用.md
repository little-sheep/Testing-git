1. `git log`查询历史版本，获取到所要回退的版本的 id
2. 恢复到某个历史版本
   `git reset --hard fae6966548e3a`
3. 将修改推送到远程服务器
   `git push -f -u origin master`

- `git reset --soft`只是回退了`git commit -m "message"`这个步骤
