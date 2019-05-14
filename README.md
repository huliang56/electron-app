# Electron React Boilerplate
<p>
  Electron React Boilerplate uses <a href="http://electron.atom.io/">Electron</a>, <a href="https://facebook.github.io/react/">React</a>, <a href="https://github.com/reactjs/redux">Redux</a>, <a href="https://github.com/reactjs/react-router">React Router</a>, <a href="http://webpack.github.io/docs/">Webpack</a> and <a href="https://github.com/gaearon/react-hot-loader">React Hot Loader</a> for rapid application development (HMR).
</p>

## Usage
```bash
# Starting Development
$ yarn dev
# Packaging for Production
$ yarn package
```

## Docs
[docs and guides](https://electron-react-boilerplate.js.org/docs/installation)

## 安装electron-react-boilerplate遇到的问题
### 一、yarn安装缓慢
```bash
# 查看下载源
yarn config get registry
# 修改下载源
yarn config set registry https://registry.npm.taobao.org
```
### 二、安装调试问题
检查系统是否已经安装好所依赖的环境（Visual C++ 和 Python 2.7）
[参考链接](https://electron-react-boilerplate.js.org/docs/installation-debugging-solutions)

若没有则以管理员身份运行 npm install --global --production windows-build-tools，安装所有使用微软的必需的工具和配置Windows的构建工具

安装好后，删除node_modules文件夹，yarn cache clean && yarn
