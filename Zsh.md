# Zsh

## 1.备忘

- zsh的配置文件加载顺序见博客：http://wxnacy.com/2018/10/08/zsh-startup-files/
- Oh-my-zsh项目的存放位置：~/.oh-my-zsh
- 已经在～中新建了.zshrc用于配置zsh，也已经将oh-my-zsh中的配置项拷贝进来
  - 修改zsh主题的方式：修改.zshrc中的ZSH_THEME，目前使用的是af-magic
  - 设置zsh的plugin的方式：修改.zshrc中的plugins=()
- 上述的zsh主题库保存在~/.oh-my-zsh/themes，各种主题截图详见https://github.com/ohmyzsh/ohmyzsh/wiki/themes
- 上述的zsh插件都保存在~/.oh-my-zsh/plugins

## 2.设置oh-my-zsh的步骤

- 从git下载oh-my-zsh

  ```shell
  git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
  ```

- 新建zsh的配置文件～/zshrc，将~/.oh-my-zsh中的配置项拷贝进～/zshrc

  ```shell
  cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
  ```

## 3.已经安装的oh-my-zsh插件

- zsh-syntax-highlighting
- zsh-autosuggestions

## 4.参考博客

- https://zhuanlan.zhihu.com/p/58073103
- https://www.jianshu.com/p/ba08713c2b19