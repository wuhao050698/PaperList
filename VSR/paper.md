# Video Super Resolution

paper|year|conference|keyword|link
-|-|-|-|-
Deep Video Super-Resolution Network Using Dynamic Upsampling Filters Without Explicit Motion Compensation|2018|CVPR|Dynamic filter network, No optical flow
TDAN: Temporally Deformable Alignment Network for Video Super-Resolution|2018|CVPR|DCN(V1)
[Data-Free Knowledge Distillation For Image Super-Resolution](#data-free-knowledge-distillation-for-image-super-resolution)|2021|CVPR|ISR, Knowledge transfer, data-free model compression|[paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_Data-Free_Knowledge_Distillation_for_Image_Super-Resolution_CVPR_2021_paper.pdf)  [code](https://github.com/twtygqyy/pytorch-vdsr)
[Unsupervised Real-World Super-Resolution: A Domain Adaptation Perspective](#unsupervised-real-world-super-resolution-a-domain-adaptation-perspective)|2021|ICCV||[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Wang_Unsupervised_Real-World_Super-Resolution_A_Domain_Adaptation_Perspective_ICCV_2021_paper.pdf)

****
## Unsupervised Real-World Super-Resolution: A Domain Adaptation Perspective
### Main idea

### Highlight

### Problem

### Idea

****
## Data-Free Knowledge Distillation For Image Super-Resolution
### Main idea
**Background**: privacy and transmission limitations

**Method**: Use the data-free compression approach in SISR. 
1. **Design a reconstruction loss for the SISR model.** Because the inputs and outputs of SR model should be in **similar distribution**. So they develop a new reconstruction loss in using this relation.
2. **Progressive Knowledge Distillation.** This mechanism will train a tiny network at first. Then they increase the number of layers and blocks gradually and train those new layers and blocks. In this way, the network can be trained easier and distill more information on intermediate features in teacher network.
   
**Experiment result**: they choose VDSR as the teacher model. The student model can achieve similar performance with the teacher model.
![](image/1.jpg)
### Highlight
Use the mechanism of progressive to solve the training difficulty of the deep network.
### Problem
1. the improvement of the progressive distillation is not significant. and they only do the ablation experiment in one dataset.
2. They did not compare the training time and parameters to show the compression.
![](image/2.jpg)
### Idea
1. In Data-Free Knowledge Distillation about VSR, we can also use the similar idea like the reconstruction loss in this paper. The inputs and outputs should be in similar distribution in the teacher model. But how to deal with the heavy model in VSR is a problem.