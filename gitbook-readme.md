## 预览指南
### 安装 nodejs 以及npm  

**Linux**  

1. `sudo apt get install nodejs-legacy`
2. `sudo apt get install npm`  

**Windows**  

通过[ nodejs 官网](https://nodejs.org/en/)下载 nodejs，windows 下自带 npm 包管理工具。

### 安装 gitbook-cli 包
Linux: `sudo npm install -g gitbook`  

windows: 管理员模式：`npm install -g gitbook`

### 安装 gitbook 相关包
切换至项目目录，运行 `gitbook install .`

### 生成 PDF
切换至项目目录，运行 `gitbook pdf`  

### 实时预览项目
切换至项目目录，运行 `gitbook serve`，浏览器打开`localhost:4000`即可边修改边预览
