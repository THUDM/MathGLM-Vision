# MathGLM-Vision
Official Pytorch Implementation for MathGLM-Vision

![](resources/perf.jpg)

Large language models (LLMs) have demonstrated significant capabilities in mathematical reasoning, particularly with text-based mathematical problems. However, current multi-modal large language models (MLLMs), especially those specialized in mathematics, tend to focus predominantly on solving geometric problems but ignore the diversity of visual information available in other areas of mathematics. Moreover, the geometric information for these specialized mathematical MLLMs is derived from several public datasets, which are typically limited in diversity and complexity. To address these limitations, we aim to construct a fine-tuning dataset named MathVL, and develop a series of specialized mathematical MLLMs termed MathGLM-Vision by conducting Supervised Fine-Tuning (SFT) on MathVL with various parameter-scale backbones. To extensively evaluate the effectiveness of MathGLM-Vision, we conduct experiments on several public benchmarks and our curated MathVL-test consisting of 2,000 problems. Experimental results demonstrate that MathGLM-Vision achieves significant improvements compared with some existing models, including backbone models and open-source mathematical MLLMs. These findings indicate the importance of diversity dataset in enhancing the mathematical reasoning abilities of MLLMs.

If you want to find the detailed introduction, Read our paper: [MathGLM-Vision: Solving Mathematical Problems with Multi-Modal Large Language Model](https://arxiv.org/pdf/2409.13729).

## Model checkpoint
The checkpoints of MathGLM-Vision-9B and MathGLM-Vision-19B are released here, which are based on GLM-4V-9B and CogVLM2 respectively.

- [MathGLM-Vision-9B checkpoint](https://huggingface.co/THUDM/MathGLM-Vision)
- [MathGLM-Vision-19B checkpoint](https://huggingface.co/THUDM/MathGLM-Vision-19B)


## Benchmark 

Our MathGLM-Vision models have achieved strong performance across various benchmarks, including MathVista, MathVerse, and MathVision. Additionally, we introduce a benchmark called MathVL-test, designed to evaluate the ability of Multi-Modal Large Language Models (MLLMs) in multimodal mathematical reasoning, specifically within the context of Chinese K12 education.

| Model               | MathVista (GPS) | MathVista | MathVerse | MathVision | MathVL-test|
|:--------------------|:----------:|:--------:|:------:|:----:|:----:|
| MathGLM-Vision-9B   |    64.42   |   52.20  |  44.20 | 19.18| 57.05 |
| MathGLM-Vision-19B  |    65.38   |   61.10  |  42.50 | 21.64| 57.30 |
| MathGLM-Vision-32B  |    62.02   |   62.40  |  49.20 | 26.51| 59.00 |


## Detailed performance
Performance on 


## Quick start



### Citation

If you find our work helpful, please consider citing the following papers

```
@article{yang2024mathglm,
  title={MathGLM-Vision: Solving Mathematical Problems with Multi-Modal Large Language Model},
  author={Yang, Zhen and Chen, Jinhao and Du, Zhengxiao and Yu, Wenmeng and Wang, Weihan and Hong, Wenyi and Jiang, Zhihuan and Xu, Bin and Dong, Yuxiao and Tang, Jie},
  journal={arXiv preprint arXiv:2409.13729},
  year={2024}
}
```
