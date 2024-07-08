<p align="center">
 <br>
 <h1 align="center">SafeAligner: Safety Alignment against Jailbreak Attacks via Response Disparity Guidance
 <!-- <br>   -->
 </h1>
</p>

<p align="center">
 <a href="https://github.com/UmeanNever/B2NER/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/UmeanNever/B2NER"></a>
 <a href="https://arxiv.org/pdf/2406.18118"><img alt="Paper" src="https://img.shields.io/badge/📖-Paper-red"></a>
 <a href="https://huggingface.co/datasets/csHuang/SafeAligner"><img alt="Data" src="https://img.shields.io/badge/📀-Data-blue"></a>
</p>

We introduce SafeAligner, a novel method to enhance the security of large language models (LLMs) against jailbreak attacks. SafeAligner uses two specially trained models—the Sentinel Model for safety and the Intruder Model for risk simulation—to improve response security dynamically during decoding. Our tests show that SafeAligner effectively balances enhanced security with maintained performance, providing a robust and efficient defense solution.

 - 📖 Paper: [SafeAligner: Safety Alignment against Jailbreak Attacks via Response Disparity Guidance](https://arxiv.org/pdf/2406.18118)
 - 🎮 Code Repo: https://github.com/csHuangfdu/SafeAligner
 - 📀 Data: You can download from [HuggingFace](https://huggingface.co/datasets/csHuang/SafeAligner).


# OverView

![Overview](figs/Figure1.png)

# Data
One of the core contributions of this paper is the construction of the SafeAligner dataset. It includes 628 English data in 8 harmful scenarios, where each data consists of a harmful query and its safe and harmful replies, as shown in the following table.

| Scenario                  | Num | # Ins | # Saf | # Haf |
|---------------------------|-----|-------|-------|-------|
| Adult Content             |  34 | 12.2  | 19.6  | 272.3 |
| Economic Harm             |  38 | 14.8  | 17.8  | 218.8 |
| Fraud Deception           |  72 | 15.1  | 20.4  | 241.1 |
| Illegal Activity          | 144 | 14.6  | 21.4  | 206.5 |
| Hate/Harass/Violence      | 130 | 15.7  | 17.3  | 183.8 |
| Malware                   | 130 | 17.0  | 20.1  | 249.3 |
| Physical Harm             |  39 | 14.1  | 19.8  | 212.4 |
| Privacy Violation Activity|  41 | 17.2  | 14.5  | 183.5 |

`Num` represents the number of statistical data entries. 
`Ins` refers to harmful queries. 
`Saf` denotes safe responses.
`Haf` indicates harmful responses. 
`#` represents the average token length.

This dataset supports future research on LLM jailbreak attacks, LLM security alignment research, etc.

# Getting Start
We will release the code after the paper is accepted ...


# Cite
```
@article{huang2024safealigner,
  title={SafeAligner: Safety Alignment against Jailbreak Attacks via Response Disparity Guidance},
  author={Huang, Caishuang and Zhao, Wanxu and Zheng, Rui and Lv, Huijie and Dou, Shihan and Li, Sixian and Wang, Xiao and Zhou, Enyu and Ye, Junjie and Yang, Yuming and others},
  journal={arXiv preprint arXiv:2406.18118},
  year={2024}
}
```