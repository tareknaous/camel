# CAMeL: Cultural Appropriateness Measure Set for LMs

<img align="center"  src="camel-pic.png" alt="camel">


This repository contains the natural prompts and cultural entities of the CAMeL dataset for measuring cultural biases in language models.

For more details, see the accompanying paper: ["Having Beer After Prayer? Measure Cultural Bias in Large Language Models"](https://arxiv.org/abs/2305.14456), **Accepted at ACL 2024**

## Prompts

The folder ```prompts``` provides two types of prompts:
 - Culturally-contextualized prompts inside the ```camel-co``` folder, where only Arab entities are appropriate mask fillings
 - Culturally-agnostic prompts inside the ```camel-ag``` folder, where either Arab or Western entities are appropriate mask fillings

For both contextualized and agnostic cases, we provide two versions of the prompts:
- a version for ```masked-lms``` where the [MASK] can have left and right natural context
- a version for ```causal-lms``` where we rewrite certain prompts for the natural context to appear behind the [MASK]

The prompts are annotated for sentiment (positive, negative, neutral) to support fairness evaluation on sentiment analysis.

## Prompts

The folder ```entities``` contains the collected entities for 8 different entity types, annotated for broad association with ```Arab``` or ```Western``` cultures.

## Citation
```
@article{naous2023having,
  title={Having beer after prayer? measuring cultural bias in large language models},
  author={Naous, Tarek and Ryan, Michael J and Ritter, Alan and Xu, Wei},
  journal={arXiv preprint arXiv:2305.14456},
  year={2023}
}
```

## Contact
**Tarek Naous**: [Scholar](https://scholar.google.com/citations?user=ImyLv44AAAAJ&hl=en) | [Github](https://github.com/tareknaous?tab=repositories) |
[Linkedin](https://www.linkedin.com/in/tareknaous/) |  [Research Gate](https://www.researchgate.net/profile/Tarek_Naous?ev=hdr_xprf) | [Personal Wesbite](https://www.sites.google.com/view/tareknaous)
| tareknaous@gatech.edu
