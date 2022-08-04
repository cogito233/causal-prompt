# llm-bivariate-causal-discovery
## Introduction
Identifying the causal direction between two variables has long been an important but challenging task for causal inference. Existing work proposes to distinguish whether $X\rightarrow Y$ or $Y \rightarrow X$ by setting up an input-output learning task using the two variables, since causal and anticausal learning have different performances under semi-supervised learning and domain shift. This approach works for many task-specific models trained on the input-output pairs. However, with the rise of general-purpose large language models (LLMs), there are various challenges posed to this previous task-specific learning approach, since continued training of LLMs is less likely to be affordable for university labs, and LLMs are no longer trained on specific input-output pairs. In this work, we propose a new paradigm to distinguish cause from effect using LLMs. Specifically, we conduct post-hoc analysis using natural language prompts that describe different possible causal stories behind the $X$, $Y$ pairs, and test their zero-shot performance. Through the experiments, we show that the natural language prompts that describe the same causal story as the ground-truth data generating direction achieve the highest zero-shot performance, with 2\% margin over anticausal prompts. We highlight that it will be an interesting direction to identify more causal relations using LLMs.

## Code Structure
