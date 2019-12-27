## Available Scripts
  just a demo to test auto deploy.

### 云服务器
  1、在服务器上面配置nginx，设置location

### 创建一个项目，并推送到github上面
  1、利用create-react-app创建一个项目
  2、本地测试完成之后推送到github上面  
  
### 了解一下Travis，https://travis-ci.com/
  1、登录官网了解基本的配置信息
  2、在项目中添加一个.travis.yml的文件
  3、在配置文件中添加自己的配置信息
      # 使用的语言
      language: node_js

      # 使用的nodejs版本
      node_js:
        - v8.17.0

      # 执行的脚本
      script:
        - npm run deploy

      # 仓库的分支
      branches:
        only:
          - master
### 登录到Travis，授权可以获取github的repositories

### 测试
    1、在本地修改完毕之后，推送到github上面
    2、在Travis上面可以查看自己的repositories，可以获取log
    3、在云服务器上面可以查看到自己的build文件（需要执行yarn run deploy,在Travis的配置上面已经执行了）
    4、可以查看到具体的页面 http://111.229.53.186/（Demo页面）