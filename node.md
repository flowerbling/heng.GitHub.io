# Node 笔记

## node换源
~~~ shell
    # npm 权限问题
    ls -la /usr/local # 查看权限
    sudo npm install xxx # 单次解决
    sudo chown -R $(whoami) $(npm config get prefix)/{lib/node_modules,bin,share} # 全局解决
    
    npm config get registry # 查看源
    npm set registry https://registry.npm.taobao.org/ # 更换淘宝源
    npm config set registry https://registry.npmjs.org # 切换为原始源
    
    # 源管理器
    npm install -g nrm
    nrm ls # 查看可选的源
    nrm use taobao # 更换淘宝源
    nrm use npm # 切换为原始源
~~~

# npm error 记录
- Cannot read properties of null (reading 'pickAlgorithm')
~~~ shell
    npm cache clear --force
~~~
