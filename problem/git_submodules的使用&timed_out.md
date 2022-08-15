submodules的使用

- 使用场景

  - You've added another git repository inside your current repository.
  - Clones of the outer repository will not contain the contents of the embedded repository and will not know how to obtain it.
  - If you meant to add a submodule, use:
    `git submodule add <url> html&css/26-Tea Station Project`

  - If you added this path by mistake, you can remove it from the
    index with:

    `git rm --cached html&css/26-Tea Station Project`

  - See "git help submodule" for more information.

- 如果push了submodules但是在github remote repository内没看到更改
  - `git submodules update`
  - 检查`.gitmodules`文件
  - `git add .`
  - `git commit -m "xxx"`
  - `git push`



问题解决

- OpenSSL SSL_read: Connection was reset, errno 10054

- Failed to connect to github.com port 443: Timed out

  - `git config --global --unset http.proxy`

  - `git config --global --unset https.proxy`

  - 换个节点





branch protection rules

- 当有一个以上的分支时需要考虑