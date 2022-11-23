# ReAct Prompting

GPT-3 prompting code for [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629).

## Setup
You need to first have an OpenAI API key and store it in the environment variable ``OPENAI_API_KEY`` (see [here](https://help.openai.com/en/articles/5112595-best-practices-for-api-key-safety)).

Package requirement: ``openai``, and install ``alfworld`` following instructions [here](https://github.com/alfworld/alfworld).

## Experiments
Run ``hotpotqa.ipynb`` and ``alfworld.ipynb``. FEVER and WebShop code will be added soon.

- On 500 random validation examples of HotpotQA, GPT-3 with ReAct prompting achieves an exact match (EM) of 30.4, while PaLM-540B is 29.4.
- On all 134 unseen validation examples of ALFWorld, GPT-3 with ReAct prompting achieves a success rate of 78.4%, while PaLM-540B is 70.9%.

## Citation

```bibtex
@article{yao2022react,
  title={{ReAct}: Synergizing Reasoning and Acting in Language Models},
  author={Yao, Shunyu and Zhao, Jeffrey and Yu, Dian and Du, Nan and Shafran, Izhak and Narasimhan, Karthik and Cao, Yuan},
  journal={arXiv preprint arXiv:2210.03629},
  year={2022}
}
```
