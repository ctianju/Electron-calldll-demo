# Electron-calldll-demo  
示例Electron 调用C的动态链接库  


dll 64位 （动态库默认是32位的，打包的时候值得注意）  

系统 Win10 64位  

问题点：  
主要是安装ffi-napi失败，环境问题，需要单独安装，并且安装的时候都勾选添加到环境变量  
---visualcppbuildtools_full.exe  
---- python-2.7.17.amd64.msi  
环境就好了，下载 npm install -g node-gyp  
紧接着下载项目依赖的 npm install --save ffi-napi  
大功告成，花了一天时间  

集成sqlite3 ，只需2步骤：  
1.npm i sqlite3 --save  
2."postinstall": "install-app-deps"  



