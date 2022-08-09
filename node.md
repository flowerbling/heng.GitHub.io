# Node 笔记

## node换源
~~~ shell
    npm config get registry # 查看源
    npm set registry https://registry.npm.taobao.org/ # 更换淘宝源
    npm config set registry https://registry.npmjs.org # 切换为原始源
    
    # 源管理器
    npm install -g nrm
    nrm ls # 查看可选的源
    nrm use taobao # 更换淘宝源
    nrm use npm # 切换为原始源
~~~
