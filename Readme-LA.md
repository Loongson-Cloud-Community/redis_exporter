### 1. 源码适配
架构无关，无需适配

### 2. 生成redis-export二进制
使用go1.19编译：   
> go env -w GOPROXY=http://goproxy.loongnix.cn:3000   
> rm -rf go.sum   
> go mod tidy //根据设定的GOPROXY源，重新生成go.sum文件   
> go mod vendor   
> go build .   
