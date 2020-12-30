# 轻量级站点部署管理工具

## 启动

```sh
cd src

# 复制配置文件
cp settings-example.py settings.py

# 配置项目及安全秘钥
vim settings.py

# 创建上传目录和模块目录
# 可以使用脚本创建(待开发)
# 创建项目目录，每个项目单独一个目录
# 说明这里的project_name对应settings.py中的项目名
mkdir /root_path/project_name
# 创建备份目录
mkdir /root_path/project_name/backup
# 创建日志目录
mkdir /root_path/project_name/logs
# 创建模块目录，每个模块单独一个目录
mkdir /root_path/project_name/module_name
# 创建模块的上传目录
# 上传的打包要发布的文件会临时保存到该目录下
mkdir /root_path/project_name/upload/module_name

# 启动
python3 main.py
```
