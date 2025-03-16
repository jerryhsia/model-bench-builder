# model-bench-builder

基于开源项目构建Docker镜像

- [https://github.com/jerryhsia/AlignBench](https://github.com/jerryhsia/AlignBench)
- [https://github.com/jerryhsia/LiveBench](https://github.com/jerryhsia/LiveBench)

# 使用方法

```bash
# docker run -d --name=modelbench -it --security-opt seccomp:unconfined jerry9916/modelbench:arm64
docker run -d --name=modelbench -it --security-opt seccomp:unconfined jerry9916/modelbench:amd64

docker exec -it modelbench bash
cd AlignBench
./run.example.sh # 按需修改变量及参数

cd liveBench
./run.example.sh # 按需修改变量及参数
```