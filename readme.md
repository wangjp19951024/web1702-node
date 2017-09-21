git
    git init
        创建一个.git文件
    git add * 
        加入git缓存
    git commit -m 'decripe'
        创建git节点(版本)
    git log
        历史节点
    git reset --hard 版本号
        版本回退
    git reflog
    git branch
        查看分支
    git branch dev
        创建分支
    git checkout dev
        切换分支
    git merge dev
        将指定分支dev合并到主分支上
    github.com

    远程仓库
        与远程仓库绑定
            git remote add origin 地址
        更新
            从远程仓库中下载内容
                git pull origin master
        本地提交
            git add *
            git commit -m ''
        远程提交
            git push origin master
            先保存在本地再远程提交
    多人协作
        发布
            git push origin master
        下载
            git clone 仓库地址



es6语法　
    ECMAScript2015
    转换工具babel
        es6--es5
    全局安装
        npm install babel-cli -g
    本地安装babel预设(转换规则)
        babel-preset-latest
        babel-preset-es2015
        babel-preset-react
        babel-preset-env
    编写配置信息
        .babelrc 放置在项目根目录下
        {
            "preset":["latest"]
        }
    使用babel进行转码
        编写es6的代码
        使用babel进行转码
            只能转换新语法，无法转码新功能
            babel hello.js --out-file out.js
        babel的本地使用
            本地安装babel-cli和babel-preset-latest
                npm install --save-dev
            添加配置信息
                vim .babelrc
                {
                    "presets":["latest"]
                }
            在package.json中添加脚本
            {
                "script":{
                    "build":"babel src --out-dir dist"
                }
            }
            执行转化
                npm run build
        变量
            let
                与var相比
                    不允许重复声明
                    没有变量提升
                    具有局部作用域
            const
                具有let所有特性
                必须显示初始化 (具体数值)
                不能二次赋值(只读)
        解构
            一个表达式可以完成多个变量的赋值操作,(模式匹配)
            １.数组解构
                var arr = [1,2,3];
                let [a,b,c] = arr;
                




    

