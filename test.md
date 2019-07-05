

```
# 本地克隆一个仓库
$ git clone https://github.com/adlovex/adlovex.github.io.git

# 检查连接状态
$ cd adlovex.github.io
$ git remote -v
origin	https://github.com/adlovex/adlovex.github.io.git (fetch)
origin	https://github.com/adlovex/adlovex.github.io.git (push)

# 将HTTPS改成SSH方式
$ git remote set-url origin git@github.com:adlovex/adlovex.github.io.git

# 查看
$ git remote -v
origin	git@github.com:adlovex/adlovex.github.io.git (fetch)
origin	git@github.com:adlovex/adlovex.github.io.git (push)

# 创建测试文件提交到远程仓库
$ touch test.md
$ git add test.md 
$ git status
$ git commit -m "fist commit test"

# 提示需要设置全局user.email和user.name，完成设置再重新提交即可
$ git config --global user.email "you@example.com"
$ git config --global user.name "Your Name"

$ git commit -m "fist commit test"
[master 8544431] fist commit test
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test.md

# 首次提交到远程GitHub仓库，需要输入SSH密码验证
$ git push origin master  
... ...
枚举对象: 4, 完成.
对象计数中: 100% (4/4), 完成.
使用 4 个线程进行压缩
压缩对象中: 100% (2/2), 完成.
写入对象中: 100% (3/3), 309 bytes | 309.00 KiB/s, 完成.
总共 3 （差异 0），复用 0 （差异 0）
To github.com:adlovex/adlovex.github.io.git
   0461554..8544431  master -> master
```

