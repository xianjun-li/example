# Protocol Buffers

## overview

是对结构化数据进行序列化的工具，语言无关，平台无关。

## Quick start

see <https://developers.google.cn/protocol-buffers/>

### install

pre-built binary compiler: <https://github.com/protocolbuffers/protobuf/releases>

go generated code
see: <https://developers.google.cn/protocol-buffers/docs/reference/go-generated>

```
$ go install google.golang.org/protobuf/cmd/protoc-gen-go
```

### generate code

```
protoc --go_out=$DST_DIR $SRC_FILE
```

e.g.

```
# change to the current file dir
# --proto_path
protoc --go_out=./helloworld --proto_path=./pb ./pb/helloworld.proto
```
