# 2021Summer-Image-Compression
An reimplement of HESIC by MindSpore



Comments 备注
```
一、compressai/layers/layers.py
1. line52
没有nn.PixelShuffle层可用


二、compressai/entropy_models/entropy_models.py
1. line141
ops.Round不支持CPU运算

2. line378 & 382
mindspore没有对Tensor进行clamp的函数

3. line737
ops.Erfc不支持CPU运算


三、compressai/ops/ops.py
1. line32
mindspore没有detach
```
