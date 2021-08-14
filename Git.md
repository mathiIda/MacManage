# Git

## 1.备忘

- Git存储位置：/usr/bin/git

## 2.配置过程

- 查看版本

  ```shell
  git --version
  ```

- 本地配置

  ```shell
  git config --global user.name=${name} #全局配置name
  git config --global user.email=${email} #全局配置email
  git config user.name=${name} #配置name
  git config user.email=${email} #配置email
  
  git config user.name #查看name
  git config user.email #查看email
  git config --global user.name #查看全局name
  git config --global user.email #查看全局email
  
  git config -l #查看所有配置
  git config --global -l #查看所有全局配置
  ```

  全局配置文件：～/.gitconfig

## 3.配置github ssh

- SSH公钥生成

  ```shell
  ssh-keygen -t rsa -C "${email}"
  ```

  详见博客：https://git-scm.com/book/zh/v2/%E6%9C%8D%E5%8A%A1%E5%99%A8%E4%B8%8A%E7%9A%84-Git-%E7%94%9F%E6%88%90-SSH-%E5%85%AC%E9%92%A5

  生成的公钥位置：~/.ssh/id_rsa.pub

  与之对应的私钥位置：~/.ssh/id_rsa

- 测试ssh连接，同时将github.com加入信任hosts

  ```shell
  ssh -T git@github.com
  ```

  成功之后会收到

  ```
  Hi mathiIda! You've successfully authenticated, but GitHub does not provide shell access.
  ```

- 可以通过ssh clone/push到github了
- 参考博客：https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh

## 4.常用命令

- 修改已经push的commit

  ```shell
  git push --force origin main
  ```

  

## 5.注意事项

- user.name="niuniu",user.email="niumengliang@tp-link.com.cn",则commiter显示为"niuniu"
- user.name="xxx",user.email="2487000318@qq.com",则不管name为何，commiter都显示为"mathiIda"

- github可以通过https的方式clone，但已经不支持通过https的方式push了
- github目前支持通过ssh的方式push/clone