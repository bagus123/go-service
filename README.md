# go-service


## Installation
```shell
# 1. clone repository
git clone https://github.com/bagus123/go-service.git

# 2. downloads all dependencies
go build

# note
# clean cache go
go clean --modcache

# remove unused module
go mod tidy
```


## How to create this module
```shell
go mod init github.com/bagus123/go-service

# add library
go get -u github.com/golang/protobuf/proto
go get -u github.com/golang/protobuf/protoc-gen-go

#compile proto
protoc --go_out=plugins=grpc:. *.proto
```