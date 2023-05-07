To install on WSL2

set cuda home

```
export CUDA_HOME=/usr/lib/wsl/lib/
```

install mmpretrain,mmengine,mmcv-full

```
pip install -e .[all]
pip install mmengine
pip install mmcv-full
```

install g++

```
sudo apt install g++
```

for libGl.so
```
apt-get update && apt-get install ffmpeg libsm6 libxext6  -y
```


test install with 
```
python demo/image_demo.py demo/demo.JPEG resnet18_8xb32_in1k --device cuda:0
```

