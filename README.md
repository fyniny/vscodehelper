# vscodehelper
vscode go语言插件 linux版本全家桶

# 使用说明
----

# 解压之后丢在gopath路径之下
> src文件太大，故采用分卷压缩形式上传，解压
> 解压gz分卷
> cat src.tar.gz* | tar zx
> tar -C ${path} -zvf src.tar.gz

**若需要重新编译，拷贝src目录到gopath路径下，执行**
```
go install github.com/ramya-rao-a/go-outline
go install github.com/acroca/go-symbols
go install golang.org/x/tools/cmd/guru
go install golang.org/x/tools/cmd/gorename
go install github.com/josharian/impl
go install github.com/rogpeppe/godef
go install github.com/sqs/goreturns
go install github.com/golang/lint/golint
go install github.com/cweill/gotests/gotests
go install github.com/nsf/gocode
go install github.com/uudashr/gopkgs/cmd/gopkgs
go install github.com/fatih/gomodifytags
go install github.com/haya14busa/goplay/cmd/goplay
go install github.com/derekparker/delve/cmd/dlv
```

**编译完毕后，若vscode仍然提示缺少gocode-gomod**
```
	cp $GOPATH/bin/gocode $GOPATH/bin/gocode-gomod
```

***若想要更新最新（需要自行解决墙的问题***
```
go get -u -v github.com/ramya-rao-a/go-outline
go get -u -v github.com/acroca/go-symbols
go get -u -v golang.org/x/tools/cmd/guru
go get -u -v golang.org/x/tools/cmd/gorename
go get -u -v github.com/josharian/impl
go get -u -v github.com/rogpeppe/godef
go get -u -v github.com/sqs/goreturns
go get -u -v github.com/golang/lint/golint
go get -u -v github.com/cweill/gotests/gotests
go get -u -v github.com/nsf/gocode
go get -u -v github.com/uudashr/gopkgs/cmd/gopkgs
go get -u -v github.com/fatih/gomodifytags
go get -u -v github.com/haya14busa/goplay/cmd/goplay
go get -u -v github.com/derekparker/delve/cmd/dlv
```

