# learn-grpc-go

## install
```bash
# install protoc
PROTOC_ZIP=protoc-3.7.1-linux-x86_64.zip
curl -OL https://github.com/protocolbuffers/protobuf/releases/download/v3.7.1/$PROTOC_ZIP
sudo unzip -o $PROTOC_ZIP -d /usr/local bin/protoc
sudo unzip -o $PROTOC_ZIP -d /usr/local 'include/*'
rm -f $PROTOC_ZIP

# install 
GO111MODULE=on go get github.com/golang/protobuf/protoc-gen-go@v1.3
export PATH="$PATH:$(go env GOPATH)/bin"
```

## ref 
- [quick start](https://grpc.io/docs/languages/go/quickstart/)
- [installing-protoc](http://google.github.io/proto-lens/installing-protoc.html/)