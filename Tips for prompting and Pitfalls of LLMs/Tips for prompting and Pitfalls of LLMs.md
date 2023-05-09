# Tips for prompting and Pitfalls of LLMs

- 1. [Tips for prompting](#Tipsforprompting)
- 2. [Pitfalls of LLMs](#PitfallsofLLMs)

## 1. <a name='Tipsforprompting'></a>Tips for prompting

1. Ask to continue if thread ends due to character limit
1. If you don't want to start a new dialog, but want the neural network not to use the previous context, write "Forget all the context above".
1. When working on text generation tasks, it's possible to use a high **temperature** or **top p** value to encourage more creative and varied outputs. However, for tasks where precision and accuracy are crucial, such as translation or question answering, it's important to use a low temperature or top p value to improve the factual correctness and overall accuracy of the output. Note: It's not possible to adjust configuration hyperparameters for certain models, such as ChatGPT, unless you use the API.

## 2. <a name='PitfallsofLLMs'></a>Pitfalls of LLMs

1. LLMs generally have difficulty accurately citing sources due to the fact that they lack access to the internet and do not possess the ability to recall the exact origins of their information. As a result, they may often generate sources that appear credible but are actually incorrect.
1. Careful fact-checking is necessary when working with LLMs because they often generate lies when they are asked a question to which they do not know the answer.
1. LLMs are usually bad at math.
