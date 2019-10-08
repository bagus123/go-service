# go-service


```shell
go mod init github.com/bagus123/go-service

# add library
go get -u github.com/golang/protobuf/proto
go get -u github.com/golang/protobuf/protoc-gen-go

#compile proto
protoc --go_out=plugins=grpc:. *.proto
```