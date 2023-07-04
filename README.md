# ReAct Prompting

GPT-3 prompting code for ICLR 2023 paper [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629).

To use ReAct for more tasks, consider trying [LangChain's zero-shot ReAct Agent](https://python.langchain.com/docs/modules/agents/agent_types/react.html).

## Setup
You need to first have an OpenAI API key and store it in the environment variable ``OPENAI_API_KEY`` (see [here](https://help.openai.com/en/articles/5112595-best-practices-for-api-key-safety)).

Package requirement: ``openai``, and install ``alfworld`` following instructions [here](https://github.com/alfworld/alfworld).

## Experiments
Run ``{hotpotqa,fever,alfworld,webshop}.ipynb``. As HotpotQA and FEVER have large validation sets, we only run 500 random examples (see notebooks). We find PaLM and GPT-3 are better at different tasks.


|                    | HotpotQA (500 random dev, EM) | FEVER (500 random dev, EM) | AlfWorld (success rate) | WebShop  (success rate) |
|--------------------|-------------------------------|----------------------------|-------------------------|-------------------------|
| PaLM-540B (paper)  | 29.4                          | 62.2                       | 70.9                    | 40                      |
| GPT-3 (davinci-002) | 30.4                          | 54                         | 78.4                    | 35.8                    |

## Citation

```bibtex
@inproceedings{yao2023react,
  title = {{ReAct}: Synergizing Reasoning and Acting in Language Models},
  author = {Yao, Shunyu and Zhao, Jeffrey and Yu, Dian and Du, Nan and Shafran, Izhak and Narasimhan, Karthik and Cao, Yuan},
  booktitle = {International Conference on Learning Representations (ICLR) },
  year = {2023},
  html = {https://arxiv.org/abs/2210.03629},
}
```
