# Prometheus

## 1.备忘

- 已通过Homebrew安装Prometheus：brew install prometheus
- Prometheus的安装路径：/opt/homebrew/Cellar/prometheus
- Prometheus的可执行文件路径：/opt/homebrew/bin/prometheus、/opt/homebrew/bin/prometool
- Prometheus的配置文件路径：/opt/homebrew/etc/prometheus.yml

## 2.常用命令

- 启动

  ```shell
  prometheus --config.file=/opt/homebrew/etc/prometheus.yml
  ```

  