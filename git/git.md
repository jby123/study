# git 忽略文件修改
    git rm --cached
    git rm -r .gitignore --cached
    git rm -r . --cached
# git submode

# git subtree
    git subtree push --prefix=dist origin gh-pages
    
    git remote add -f <子仓库名> <子仓库地址>
    git remote add -f libpng https://github.com/test/libpng.git
    
    git subtree add --prefix=<子目录名> <子仓库名> <分支> --squash
    git subtree add --prefix=sub/libpng libpng master --squash
    
    git fetch <远程仓库名> <分支>
    git fetch libpng master
    
    git subtree pull --prefix=<子目录名> <远程分支> <分支> --squash
    git subtree pull --prefix=sub/libpng https://github.com/test/libpng.git master --squash