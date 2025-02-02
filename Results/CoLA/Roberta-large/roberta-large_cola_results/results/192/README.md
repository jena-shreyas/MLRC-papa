---
language:
- en
license: mit
tags:
- generated_from_trainer
datasets:
- glue
metrics:
- matthews_correlation
model-index:
- name: output
  results:
  - task:
      name: Text Classification
      type: text-classification
    dataset:
      name: GLUE COLA
      type: glue
      args: cola
    metrics:
    - name: Matthews Correlation
      type: matthews_correlation
      value: 0.48480331556829936
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [roberta-large](https://huggingface.co/roberta-large) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5065
- Matthews Correlation: 0.4848

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 2e-05
- train_batch_size: 32
- eval_batch_size: 32
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: constant
- num_epochs: 15.0

### Training results

| Training Loss | Epoch | Step | Validation Loss | Matthews Correlation |
|:-------------:|:-----:|:----:|:---------------:|:--------------------:|
| No log        | 1.0   | 268  | 0.5431          | 0.2935               |
| 0.4979        | 2.0   | 536  | 0.5351          | 0.3815               |
| 0.4979        | 3.0   | 804  | 0.5083          | 0.4030               |
| 0.4295        | 4.0   | 1072 | 0.4740          | 0.4248               |
| 0.4295        | 5.0   | 1340 | 0.5139          | 0.4189               |
| 0.4122        | 6.0   | 1608 | 0.5234          | 0.4284               |
| 0.4122        | 7.0   | 1876 | 0.5195          | 0.4231               |
| 0.3904        | 8.0   | 2144 | 0.5078          | 0.4510               |
| 0.3904        | 9.0   | 2412 | 0.4863          | 0.4601               |
| 0.3726        | 10.0  | 2680 | 0.5216          | 0.4332               |
| 0.3726        | 11.0  | 2948 | 0.4664          | 0.4894               |
| 0.3661        | 12.0  | 3216 | 0.5172          | 0.4900               |
| 0.3661        | 13.0  | 3484 | 0.4602          | 0.4918               |
| 0.3512        | 14.0  | 3752 | 0.5370          | 0.4493               |
| 0.341         | 15.0  | 4020 | 0.5065          | 0.4848               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
