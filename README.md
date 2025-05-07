# Alpha-SQL: Zero-Shot Text-to-SQL using Monte Carlo Tree Search

This is the homepage for our ICML 2025 paper "Alpha-SQL: Zero-Shot Text-to-SQL using Monte Carlo Tree Search".

## Overview

Text-to-SQL, which enables natural language interaction with databases, serves as a pivotal method across diverse industries. With new, more powerful large language models (LLMs) emerging every few months, fine-tuning has become incredibly costly, labor-intensive, and error-prone. As an alternative, zero-shot Text-to-SQL, which leverages the growing knowledge and reasoning capabilities encoded in LLMs without task-specific fine-tuning, presents a promising and more challenging direction.

To address this challenge, we propose **Alpha-SQL**, a novel approach that leverages a Monte Carlo Tree Search (MCTS) framework to iteratively infer SQL construction actions based on partial SQL query states. To enhance the framework's reasoning capabilities, we introduce LLM-as-Action-Model to dynamically generate SQL construction actions during the MCTS process, steering the search toward more promising SQL queries. Moreover, Alpha-SQL employs a self-supervised reward function to evaluate the quality of candidate SQL queries, ensuring more accurate and efficient query generation.

Experimental results show that Alpha-SQL achieves 69.7% execution accuracy on the BIRD development set, using a 32B open-source LLM without fine-tuning. Alpha-SQL outperforms the best previous zero-shot approach based on GPT-4o by 2.5% on the BIRD development set.

## Citation

If you find our work useful, please cite our paper:

```bibtex
@inproceedings{alpha-sql,
      author       = {Boyan Li and
                      Jiayi Zhang and
                      Ju Fan and
                      Yanwei Xu and
                      Chong Chen and
                      Nan Tang and
                      Yuyu Luo},
      title        = {Alpha-SQL: Zero-Shot Text-to-SQL using Monte Carlo Tree Search},
      booktitle    = {Forty-Second International Conference on Machine Learning, {ICML} 2025,
                      Vancouver, Canada, July 13-19, 2025},
      publisher    = {OpenReview.net},
      year         = {2025}
}
```

## Links

- [Paper](https://arxiv.org/pdf/2502.17248)
- [arXiv](https://arxiv.org/abs/2502.17248)
- [Code](https://github.com/HKUSTDial/Alpha-SQL)
