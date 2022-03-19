# Note for Video Super Resolution


## Method Comparison

Model|Alignment|Params(M)|Runtime(ms)|REDS4(PSNR)
-|-|-|-|-
ToFlow|Optical Flow|||27.98|
DUF|Dynamic Upsampling Filters|Sliding window|5.8|974|28.63|
TDAN|DCN(V1)|Sliding window||||
EDVR|DCN(V2) + Temporal and Spatial Attention|Sliding window|20.6|378|31.09|
BasicVSR|Optical flow|Bi-RNN|6.3|63|31.42|
BasicVSR++|Optical flow + DCN|Second-order grid propagation|7.3|77|32.39|
VRT|Optical flow + Self-attention|Shifted window|35.6|243|32.19|

(ref:experiment result for [VRT](paper.md#VRT:+A+Video+Restoration+Transformer))

## Outline
<img src="image/n1.jpg" width="100%" />
