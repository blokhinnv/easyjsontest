# easyjsontest

cd demo
go mod init demo
<!-- на всякий случай попробую удалить -->
<!-- go clean -i easyjson -->
<!-- package easyjson is not in GOROOT (C:\Program Files\Go\src\easyjson) -->
go get github.com/mailru/easyjson && go install github.com/mailru/easyjson/...@latest
<!-- go: added github.com/josharian/intern v1.0.0
go: added github.com/mailru/easyjson v0.7.7 -->
easyjson -all task9.go
<!-- don't know how to decode string
exit status 1
Bootstrap failed: exit status 1 -->


OS: Win 10 Pro 21H2
GO: 1.19
<!-- go env
set GO111MODULE=on
set GOARCH=amd64
set GOBIN=
set GOCACHE=C:\Users\Nikita\AppData\Local\go-build
set GOENV=C:\Users\Nikita\AppData\Roaming\go\env
set GOEXE=.exe
set GOEXPERIMENT=
set GOFLAGS=
set GOHOSTARCH=amd64
set GOHOSTOS=windows
set GOINSECURE=
set GOMODCACHE=C:\Users\Nikita\go\pkg\mod
set GONOPROXY=
set GONOSUMDB=
set GOOS=windows
set GOPATH=C:\Users\Nikita\go
set GOPRIVATE=
set GOPROXY=https://proxy.golang.org,direct
set GOROOT=C:\Program Files\Go
set GOSUMDB=sum.golang.org
set GOTMPDIR=
set GOTOOLDIR=C:\Program Files\Go\pkg\tool\windows_amd64
set GOVCS=
set GOVERSION=go1.19.1
set GCCGO=gccgo
set GOAMD64=v1
set AR=ar
set CC=gcc
set CXX=g++
set CGO_ENABLED=1
set GOMOD=E:\go\easyjsontest\demo\go.mod
set GOWORK=
set CGO_CFLAGS=-g -O2
set CGO_CPPFLAGS=
set CGO_CXXFLAGS=-g -O2
set CGO_FFLAGS=-g -O2
set CGO_LDFLAGS=-g -O2
set PKG_CONFIG=pkg-config
set GOGCCFLAGS=-m64 -mthreads -Wl,--no-gc-sections -fmessage-length=0 -fdebug-prefix-map=C:\Users\Nikita\AppData\Local\Temp\go-build3683704422=/tmp/go-build -gno-record-gcc-switches -->
