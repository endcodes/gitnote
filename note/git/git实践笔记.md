# git实践笔记

## git配置

##### 首次安装git时需设置用户信息

```shell
git config --global user.name [用户名]
git config --global user.email [用户邮箱]
```

##### 查看git环境详细配置

```shell
# 查看全部配置信息
git config -l
# 查看系统配置
git config --system --list
# 查看当前用户(global)配置
git config --global --list
# 查看当前仓库配置
git config --local --list
```

##### 新代码库的初始化

```shell
# 已在代码库的目录下
git init
# 新建一个目录，将其初始化为git代码库
git init [代码库名称]
```

##### 克隆远程仓库

```shell
git clone [远程仓库地址]
```

##### 添加远程仓库地址

```shell
git remote add origin [远程仓库地址]
```

##### 提交代码至远程仓库

```shell
git push -u origin [分支名]
```

