# myQuery.js – 大道至简，我用myQuery

[![](https://img.shields.io/badge/myQuery-up--to--date-green.svg)](https://github.com/moyu-edu/myQuery/issues) [![](https://img.shields.io/badge/license-GPL3.0-green.svg)](https://github.com/moyu-edu/myQuery/blob/master/LICENSE)
```
     ___  ___  __    __  _____     _   _   _____   _____   __    __ 
    /   |/   | \ \  / / /  _  \   | | | | | ____| |  _  \  \ \  / / 
   / /|   /| |  \ \/ /  | | | |   | | | | | |__   | |_| |   \ \/ /  
  / / |__/ | |   \  /   | | | |   | | | | |  __|  |  _  /    \  /   
 / /       | |   / /    | |_| |_  | |_| | | |___  | | \ \    / /    
/_/        |_|  /_/     \_______| \_____/ |_____| |_|  \_\  /_/     

```

## 安装

### 确保您安装了npm

在cmd命令行中执行`npm -v`如果没有报错提示的是npm版本信息，则说明您已安装了npm,否则请到[nodejs官网](http://nodejs.org)。

### 国内用户还需要配置taobao源

```
    npm install -g cnpm --registry=https://registry.npm.taobao.org
```

### 第一步

#### npm方式

```
    npm install myquery  
```

#### git方式

```
    git clone https://github.com/moyu-edu/myQuery.git
```

#### 直接下载

[点这里](https://github.com/moyu-edu/myQuery/zipball/master)

### 第二步

解压到工作目录中，执行
```
    cnpm install
```

### 第三步
执行gulp dev，把您的html,js,css文件扔到examples文件夹下面，然后开始访问，地址格式如下:
```
    http://localhost/你的文件名
```

注意，如果您的端口80被占用了，有可能会出问题，请自行修改gulpfile.js里的端口配置，或到github上给作者提issue.

## 常用命令
- `gulp dev` 开发的时候访问
- `gulp devsass` 适合使用sass的用户
- `gulp devless` 适合使用less的用户
- `gulp` 上线版本执行的命令，会进行eslint检测并进行压缩代码，如果执行成功可以到dist文件夹中看到您的js压缩代码
- `gulp postcss` 自动加前缀等


## ajax相关
如果要fixture(mock,伪造)数据，请到这里生成[generate](http://www.generatedata.com/)好[不明白为什么这么优秀的作品国内没多少人用，真的比那些mock.js好用多了]，在examples文件中新建一个json.txt,把json数据放进去并保存，然后就可以在您的项目中用ajax请求这个假数据了。

## 单元测试
使用qunit进行测试，默认集成到了开发环境中，请参考demo使用在您的项目中
![qunit](http://7xp6ta.com1.z0.glb.clouddn.com/qunit.png)

## 更多信息

访问[myQuery官网](http://moyu-edu.github.io/myQuery/) 

## 为什么不像其他的工具一样考虑实现配置代理?
越是复杂的npm包越是难以安装成功，对机器的性能配置要求高，再加上GFW，我认为完全没有必要把代理集成进来，其实最简单办法是用fiddler2或charles来做代理。

## 授权

myQuery.js 遵守GPL3.0协议
