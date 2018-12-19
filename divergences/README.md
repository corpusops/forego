# Add binary release

```
docker run -it  --rm -v $(pwd):/go/src/forego -w /go/src/forego  golang bash -c 'echo $GOPATH && go get && make'
```
then upload where you want ``./forego``
