# grpc gateway csv marshaler

This is an implementation of the
[runtime.Marshaler](https://godoc.org/github.com/grpc-ecosystem/grpc-gateway/runtime#Marshaler)
interface marshaling responses to csv.

You might register the marshaler using

```
mux := runtime.NewServeMux(runtime.WithMarshalerOption("text/csv", &csv.Marshaler{}))
```

Documentation on grpc-gateway custom marshalers may be found [here](https://github.com/grpc-ecosystem/grpc-gateway/blob/master/docs/_docs/customizingyourgateway.md).