# deepcopy
a incremental backup tool based on docker

这是一个非常原始的版本，如果你需要使用该工具来备份你的文件系统，那么你需要修改main函数中备份文件路径（/home/xuriwuyun)和你想要写入的目标文件路径（/media/xuriwuyun/新加卷1/home/)
它依赖于docker提供的包，所以需要下载docker源码文件。将docker放在~/go/src/github.com/docker/目录下，执行如下命令运行：
sudo GOPATH=~/go:~/go/src/github.com/docker/docker/vendor/ go run deepcopy.go
如果备份文件目录较大，那么该工具运行时间较多，我的环境中文件目录大小在200G，运行时间大概为1小时。
