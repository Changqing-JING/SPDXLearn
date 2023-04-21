# Generate spdx from a cmake project
```shell
git submodule update --init
mkdir -p ./build/.cmake/api/v1/query
touch ./build/.cmake/api/v1/query/codemodel-v2
cmake -B build .
mkdir spdx
python cmake-spdx/main.py ./build/.cmake/api/v1/reply/$(ls ./build/.cmake/api/v1/reply | grep index) ./spdx SPDXLearn
```

# Generate spdx with spdx-tools
```shell
pip install spdx-tools
python ./generate_spdx.py spdx/Hello_SPDX.spdx
```