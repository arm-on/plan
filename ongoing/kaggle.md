[Go Back](https://github.com/arm-on/plan/blob/main/README.md)

# Kaggle

## Hindi-Tamil QA

Deadline: Nov 9, 2021
<img src="http://gen.sendtric.com/countdown/28vagyjlv6" style="display:block;">

To do:
- QA in BERT Models
- What is XLM
- Is QA using XLM, the same as it with BERT?

Problem:
- When running `trainer.train()`, I got an error:

`RuntimeError: The expanded size of the tensor (14991) must match the existing size (514) at non-singleton dimension 1.  Target sizes: [16, 14991].  Tensor sizes: [1, 514]`

Reading:

1. https://yashuseth.blog/2019/06/12/bert-explained-faqs-understand-bert-working/


MLM Code:
https://github.com/google-research/bert/blob/0fce551b55caabcfba52c61e18f34b541aef186a/create_pretraining_data.py#L342