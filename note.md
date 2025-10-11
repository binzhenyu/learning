# 各种工具学习笔记
 ## 1.git学习笔记 ##
**git——免费开源的版本控制工具。**
* 准备工作
    1. 下载git
    2. 注册github账号 
* 生成ssh密钥对
    1. 检查本地主机是否存在ssh-key命令查看本地主机是否存在ssh密钥对
        * 使用命令

            `cd ~/.ssh·`

            `ls`

    
    2. 生成ssh-key
        * 使用命令

           `ssh-keygen -t rsa -C "xxx@xxx.com"`

            
           `//执行后一直回车即可`
    3. 获取ssh-key 公钥内容（id_rsa.pub） 
        * 使用命令
            
            ```cat id_rsa.pub```

            //复制内容提交到github中
    4. 验证ssh连接是否设置成功
             
        * 使用命令
            
            `ssh -T git@github.com`
    5. 初始化本地仓库
        * 命令

            `git init`

            `git add .`

            `git commit -m 'xxx'`

    6. 将本地仓库连接远程仓库
        * 命令

            `git remote add xxx xxx.git` 
    7. 代码推送

        `git push`xxx（库） xxx（分支）          