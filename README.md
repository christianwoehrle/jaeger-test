# Sample for using Jaeger with Go

* creates spans
* porpagetes spans via remote calls
* logs events to jaeger
* emits metrics


## Setup

### start cluster
first start kind with a local registry for faster build/deployment cycles

see https://raw.githubusercontent.com/tilt-dev/kind-local/master/kind-with-registry.sh
```
./kind-with-registry.sh
```

### start tilt

```
tilt up
```


#ttps://github.com/tilt-dev/tilt-extensions/tree/master/pack
kubectl run --generator=run-pod/v1 tmp-shell --rm -i --tty --image nicolaka/netshoot -- /bin/bash

