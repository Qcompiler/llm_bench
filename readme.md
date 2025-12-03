# 代码解读

这个代码目录主要给出了如何使用opencompass评测框架， 使用标准的数据集进行评测。

```
pip install -U opencompass
opencompass --models hf_internlm2_5_1_8b_chat --datasets demo_gsm8k_chat_gen
```


# 数据集社区

包括但远不限于 
``` humaneval, triviaqa, commonsenseqa, tydiqa, strategyqa, cmmlu, lambada, piqa, ceval, math, LCSTS, Xsum, winogrande, openbookqa, AGIEval, gsm8k, nq, race, siqa, mbpp, mmlu, hellaswag, ARC, BBH, xstory_cloze, summedits, GAOKAO-BENCH, OCNLI, cmnli ```

https://hub.opencompass.org.cn/home/

# 集成已有的推理框架

你可以使用vllm等推理框架进行推理， 并使用标准的评测框架进行评测。

# 集成新的模型

在目录 configs 下， 给出了的代码示例， 你可以参考这个代码示例， 集成新的模型。

# 集成新的量化算法

在目录 configs 下， 我们给出了 llama_eval_gsm8k-mixq8.py 的代码示例， 你可以参考这个代码示例， 集成新的量化算法。