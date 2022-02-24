# ProtoBuf-test

# Install ProtoBuf
pip install protobuf    # 安装protobuf库
sudo apt-get install protobuf-compiler  # 安装protobuf编译器

# Compile proto script
## python
protoc --proto_path=[srcDir] --python_out=[outDir] [proto-script]
protoc --proto_path=./ --python_out=./python my.helloworld.proto

## javascript
protoc --proto_path=./ --js_out=import_style=commonjs,binary:./js my.helloworld.proto