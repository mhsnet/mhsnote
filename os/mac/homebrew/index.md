# [《MHS笔记》] > [《Homebrew使用》]

## 使用
```
# 查询可用包
$ brew search <pkg>
# 查看包信息
$ brew info <pkg>
# 安装包
# 例：$ brew install node@12
$ brew install <pkg>
# 删除包
$ brew uninstall <pkg>
# 设置链接
# 例：brew link --overwrite -f node@12
$ brew link <pkg@n>
# 删除链接
$ brew unlink <pkg@n>
# 已安装列表
$ brew list
# 帮助信息
$ brew -h
# 查看Homebrew版本
$ brew -v
# 更新Homebrew
$ brew update
# 体检
$ brew doctor
```

## 替换源
```
$ git -C "$(brew --repo)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git

$ git -C "$(brew --repo homebrew/core)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git

$ git -C "$(brew --repo homebrew/cask)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-cask.git

$ brew update
```

## 恢复源
```
$ git -C "$(brew --repo)" remote set-url origin https://github.com/Homebrew/brew.git

$ git -C "$(brew --repo homebrew/core)" remote set-url origin https://github.com/Homebrew/homebrew-core.git

$ git -C "$(brew --repo homebrew/cask)" remote set-url origin https://github.com/Homebrew/homebrew-cask.git

$ brew update
```

## 
[《MHS笔记》]: https://mhsnet.github.io/mhsnote/ "《MHS笔记》"

[《Homebrew使用》]: https://mhsnet.github.io/mhsnote/os/mac/homebrew/index.html "《Homebrew使用》"