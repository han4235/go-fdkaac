# go-fdkaac

Golang binding for lib-fdkaac(https://github.com/winlinvip/fdk-aac)

## Usage

First, get the source code:

```
go get -d github.com/winlinvip/go-fdkaac
```

Then, compile the fdk-aac:

```
cd $GOPATH/src/github.com/winlinvip/go-fdkaac &&
git clone https://github.com/winlinvip/fdk-aac.git &&
cd fdk-aac/ && bash autogen.sh && ./configure --prefix=`pwd`/objs && make && make install &&
cd ..
```

Done, import and use the package:

* [aac decoder](dec/example_test.go), decode the aac frame to PCM samples.

To run all examples:

```
cd $GOPATH/src/github.com/winlinvip/go-fdkaac && go test ./...
```

Winlin 2016