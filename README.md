# resv-exe

1.下载该项目：
2.renderer.js就是html页面用到的js,按照前端习惯，应放统一放在js文件夹下，且需要改名
3.js、css、html完成后,运行验证无误开始electron打包
4.安装electron及相关依赖包：项目文件夹下，命令行运行 “npm install”（这里很有可能会遇到electron安装不上的问题，多半是由于网络问题造成的，如果安装不上electron，就手动安装它，执行“npm install electron”当然，淘宝镜像也可以：cnpm install electron）
5.安装完electron后，执行 npm start,看看是否会打开窗口，会打开，证明安装无误
6.执行 electron-packager . yourpro --out ../electron  （打包生成exe文件，“yourpro”就是生成的目标项目文件夹名，不同系统系统会自动加上后缀，我的是“-win32-x64”），../electron是目标文件夹位置相对路径
7.到目标文件夹下运行yourpro.exe文件，测试效果。

附：
源代码文件夹下的main.js中，是electron构建工具的核心控制文件，其中注释已经很详细了，如需调试，可在其中进行相关配置。
