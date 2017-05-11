## 预览指南
### 安装 nodejs 以及npm  

**Linux**  

1. `sudo apt get install nodejs-legacy`
2. `sudo apt get install npm`  

**Windows**  

通过[ nodejs 官网](https://nodejs.org/en/)下载 nodejs，windows 下自带 npm 包管理工具。

### 安装 gitbook-cli 包
Linux: `sudo npm install -g gitbook-cli`  

windows: 管理员模式：`npm install -g gitbook-cli`

### 安装 gitbook 相关包
切换至项目目录，运行 `gitbook install .`

### 生成 PDF
切换至项目目录，运行 `gitbook pdf`  

### 实时预览项目
切换至项目目录，运行 `gitbook serve`，浏览器打开`localhost:4000`即可边修改边预览

**注意：由于版本Bug,windows下运行此命令会报错，需要修改以下文件**

 修改`~/.gitbook/versions/3.2.2/lib/output/website/copyPluginAssets.js`第 112 行  

 ```js
  return fs.copyDir(
        assetsFolder,
        assetOutputFolder,
        {
            deleteFirst: false,
            overwrite: true,
            confirm: false//这里改为false
        }
    );
```

**注意：由于版本 bug，windows下运行`gitbook serve`不能支持实时修改预览**