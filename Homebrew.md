# Homebrew

## 1.备忘

- Homebrew官网：https://brew.sh/

- Homebrew的安装命令：

  ```shell
  # 国内网络原因不能访问
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  # 可以正常访问的链接
  /bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
  ```

- Homebrew的卸载命令详见博客

- Homebrew的安装位置：/opt/homebrew

- 使用Homebrew install的软件的位置：/opt/homebrew/Cellar/

- 通过Homebrew安装的软件会在/opt/homebrew/bin中生成软连接，指向该软件的真实存储位置

## 2.常用命令

- 安装软件

  ```shell
  brew install ${name}
  ```

- 本地软件库列表

  ```shell
  brew ls
  ```

- 查找软件

  ```shell
  brew search ${name}
  ```

- 安装cask软件

  ```shell
  brew install --cask ${name}
  ```

- 查看版本

  ```shell
  brew -v
  ```

- 更新软件库

  ```shell
  brew update
  ```

- 查看本地过期软件列表

  ```shell
  brew outdated
  ```

## 3.知识点

- brew主要用来下载一些不带界面的命令行下的工具和第三方库来进行二次开发；
  brew cask主要用来下载一些带界面的应用软件，下载好后会自动安装，并能在mac中直接运行使用

## 4.参考博客

- https://zhuanlan.zhihu.com/p/111014448

