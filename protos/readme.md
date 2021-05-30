use `protoc` and `protoc-gen-grpc-web`

```
protoc greet.proto --js_out=import_style=commonjs:CHANGE_TO_SCRIPTS_DIRECTORY --grpc-web_out=import_style=commonjs,mode=grpcwebtext:CHANGE_TO_SCRIPTS_DIRECTORY --plugin=protoc-gen-grpc-web=CHANGE_TO_PROTOC_GEN_GRPC_WEB_EXE_PATH

protoc greet.proto --js_out=import_style=commonjs:. --grpc-web_out=import_style=commonjs,mode=grpcwebtext:. --plugin=protoc-gen-grpc-web=%protoc%\protoc-gen-grpc-web.exe
```