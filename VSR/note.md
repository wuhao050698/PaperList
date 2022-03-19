# Note for Video Super Resolution


## Method Comparison

Model|year|Alignment|Propagation|Params(M)|Runtime(ms)|REDS4(PSNR)
-|-|-|-|-|-|-|
ToFlow|2017|Optical Flow|-|-|27.98|-|
[DUF](paper.md#duf)|2018|Dynamic Upsampling Filters|Sliding window|5.8|974|28.63|
TDAN|2018|DCN(V1)|Sliding window|-|-|-|
EDVR|2020|DCN(V2) + Temporal and Spatial Attention|Sliding window|20.6|378|31.09|
BasicVSR|2021|Optical flow|Bi-RNN|6.3|63|31.42|
BasicVSR++|2021|Optical flow + DCN|Second-order grid propagation|7.3|77|32.39|
VRT|2022|Optical flow + Self-attention|Shifted window|35.6|243|32.19|

(Ref:experiment result from [VRT](paper.md#VRT))

## Outline
<img src="image/n1.jpg" width="100%" />

## Video super resolution
<img src="image/n2.jpg">

### Alignment

#### alignment
- Optical flow
- Dynamic Upsampling Filters
- Deformable Convolution Network
- Self-attention

#### propagation
- Sliding window
- RNN
- Shifted window

### Challenge and Solution
