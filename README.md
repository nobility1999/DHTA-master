# Targeted Attack for Deep Hashing based Retrieval
This repository provides implementatin our ECCV 2020 work: Targeted Attack for Deep Hashing based Retrieval.

## Abstract
The deep hashing based retrieval method is widely adopted in large-scale image and video retrieval. However, there is little investigation on its security. In this paper, we propose a novel method, dubbed deep hashing targeted attack (DHTA), to study the targeted attack on such retrieval. Specifically, we first formulate the targeted attack as a \emph{point-to-set} optimization, which minimizes the average distance between the hash code of an adversarial example and those of a set of objects with the target label. Then we design a novel \emph{component-voting scheme} to obtain an \emph{anchor code} as the representative of the set of hash codes of objects with the target label, whose optimality guarantee is also theoretically derived. To balance the performance and perceptibility, we propose to minimize the Hamming distance between the hash code of the adversarial example and the anchor code under the $\ell^\infty$ restriction on the perturbation. Extensive experiments verify that DHTA is effective in attacking both deep hashing based image retrieval and video retrieval. 


The pretrained hashing model: [VGG11_32_for_IamgeNet](https://drive.google.com/file/d/1V6Nvr0DMhquqWwsl1CQtv0Kug7aXXTzx/view?usp=sharing)

Download and save this model at "models/imagenet_vgg11_32"

Run the below command to reproduce our result.

```shell
python attack_imagenet.py --root [imagent-data-root] --reproduce --gpu-id [gpu-id]
```

The detail README is coming soon...

