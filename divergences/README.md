# Add binary release

```
w=$(id -u):$(id -g) && docker run -it  --rm -v $(pwd):/go/src/forego -w /go/src/forego  golang bash -c "rm -f forego forego.gz && go get && make && chown $w forego"  && gzip forego
```
then upload where you want ``./forego.gz``
