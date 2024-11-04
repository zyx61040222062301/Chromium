# Chromium 公共镜像使用方法
1. 将镜像文件完全解压至自己的硬盘上；
2. 将文件夹 chromium.git 重命名为 .git 并放在 chromium 文件夹中；
3. 运行以下代码以更新仓库为最新版本：
   1. 如果你想保留仓库为镜像仓库，请执行此命令：
   
      ```bash
      cd chromium
      git fetch
      ```
   2. 如果你想在更新仓库时将 master 分支中的代码取出，请将 .git 中的 config 文件替换此仓库的 config 文件，再执行以下命令：
      ```bash
      cd chromium
      git checkout master
      git pull
      ```
      或先执行 `git fetch` 更新代码变动再使用` git merge main`更新代码以代替`git pull`;
