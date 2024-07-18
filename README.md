# [AAAI 2023 Oral] FRPT
### Author: Shijie Wang, Jianlong Chang, Zhihui Wang, Haojie Li, Wanli Ouyang, Qi Tian

## Framework
![image](https://github.com/Pual2013/FRPT/blob/main/FRPT.png)

## Paper
https://arxiv.org/abs/2207.14465

## Abstrst 
Fine-grained object retrieval aims to learn discriminative representation to retrieve visually similar objects. However, existing top-performing works usually impose pairwise similarities on the semantic embedding spaces or design a localization sub-network to continually fine-tune the entire model in limited-data regimes, thus resulting in easily converging to suboptimal solutions. In this paper, we develop Fine-grained Retrieval Prompt Tuning (FRPT), which steers a frozen pre-trained model to perform the fine-grained retrieval task from the perspectives of sample prompt and feature adaptation. Specifically, FRPT only needs to learn fewer parameters in the prompt and adaptation instead of fine-tuning the entire model, thus solving the convergence to suboptimal solutions caused by fine-tuning the entire model.Technically, a discirmiantive perturbation prompt (DPP) is introduced and deemed as a sample prompt process, which amplifies and even exaggerates some discriminative elements contributing to category prediction via a content-aware inhomogeneous sampling. In this way, DPP can make the fine-grained retrieval task aided by the perturbation prompts close to the solved task during the original pre-training, thus preserving the generalization and discrimination of representation extracted from input samples.Besides, a category-specific awareness head is proposed and regarded as feature adaptation, which removes the species discrepancies in features extracted by the pre-trained model using category-guided instance normalization, and thus makes the optimized features only include the discrepancies among subcategories.Extensive experiments demonstrate that our FRPT with fewer learnable parameters achieves the state-of-the-art performance on three widely-used fine-grained datasets.
