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
        ![](./jpg/查看本地主机是否存在ssh密钥.png)
    2. 生成ssh-key
        * 使用命令

           `ssh-keygen -t rsa -C "xxx@xxx.com"`

            
           `//执行后一直回车即可`
* 获取ssh-key 公钥内容（id_rsa.pub） 
     * 使用命令
            
         ```cat id_rsa.pub```

          //复制内容提交到github中
* 验证ssh连接是否设置成功
             
     * 使用命令
            
        `ssh -T git@github.com`
* 初始化本地仓库
     * 命令

         `git init`

* 将代码推送至本地git库            

    * 命令   
        `git add .`

* 将本地更改推送至暂存

    * 命令

        `git commit -m 'xxx'`

* 将本地仓库连接远程仓库
    * 命令

         `git remote add`xxx//名称 xxx.git//远程库ssh地址

* 代码拉取
    * 命令

        `git pull`xxx//库 xxx//分支
                
* 代码推送
     * 命令
        
        `git push`xxx//库 xxx//分支          

