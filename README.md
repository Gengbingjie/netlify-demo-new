注：此demo只包含nodejs接口部分内容，不含前端页面相关代码逻辑
1、下载demo文件
    git clone git@git.code.tencent.com:gengbingjie/netlify-demo.git
    mv netlify-demo new-name
    cd new-name
    git remote set-url origin <新的远程仓库地址> (git remote add origin <新的远程仓库地址>)
    
2、安装依赖
    npm install
3、安装netlify cli（nodejs版本需在18.14.0及以上）（已安装过请忽略）
    npm install netlify-cli -g

4、发布部署
4.1、可以将项目上传到github后手动在netlify平台创建站点
    使用github进行部署，连接到git仓库

4.2、初始化netlify项目
    netlify init
        选择  Create & configure a new site
        依次选择并回车可以看到生成的 Admin URL、URL、Site ID，会自动link到新的netlify项目
        选择从github自动部署时 注意git远程仓库地址
        在github上手动添加命令行中生成的密钥

4.3、也可直接将项目文件拖到netlify平台上,使用手动部署
    netlify deploy
    netlify deploy --prod     //部署并发布


5、启动本地netlify项目
    netlify dev
    



 Netlify 操作文档 https://docs.netlify.com/functions/lambda-compatibility/

* 安装 Netlify CLI - https://docs.netlify.com/cli/get-started/