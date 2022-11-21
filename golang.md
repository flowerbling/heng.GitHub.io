# go get
~~~ shell
-d 只下载不安装
-f 只有在你包含了 -u 参数的时候才有效，不让 -u 去验证 import 中的每一个都已经获取了，这对于本地 fork 的包特别有用
-fix 在获取源码之后先运行 fix，然后再去做其他的事情
-t 同时也下载需要为运行测试所需要的包
-u 强制使用网络去更新包和它的依赖包
-v 显示执行的命令

~~~

# go command line arguments 的使用 GO中命令行参数的传递

os.Args的第一个元素，os.Args[0], 是命令本身的名字；其它的元素则是程序启动时传给它的参数。
~~~ golang
package main

import (
	"fmt"
	"os"
)

func main() {
	fmt.Println(os.Args)
}

# [/var/folders/s1/1pfsrqds1p9fcg82xzzn8zq00000gn/T/go-build3034726544/b001/exe/main hello]
~~~
