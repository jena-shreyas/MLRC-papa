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
      value: 0.08530885680462096
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5977
- Matthews Correlation: 0.0853

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
- train_batch_size: 16
- eval_batch_size: 16
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: constant
- num_epochs: 15.0

### Training results

| Training Loss | Epoch | Step | Validation Loss | Matthews Correlation |
|:-------------:|:-----:|:----:|:---------------:|:--------------------:|
| 0.6085        | 1.0   | 535  | 0.6154          | 0.0                  |
| 0.595         | 2.0   | 1070 | 0.6058          | 0.0                  |
| 0.5959        | 3.0   | 1605 | 0.6101          | 0.0                  |
| 0.5848        | 4.0   | 2140 | 0.5948          | 0.1039               |
| 0.5887        | 5.0   | 2675 | 0.5939          | 0.0686               |
| 0.5834        | 6.0   | 3210 | 0.6123          | 0.0181               |
| 0.5782        | 7.0   | 3745 | 0.6104          | 0.0467               |
| 0.573         | 8.0   | 4280 | 0.6132          | 0.0467               |
| 0.5765        | 9.0   | 4815 | 0.5985          | 0.0551               |
| 0.5695        | 10.0  | 5350 | 0.6068          | 0.0717               |
| 0.5617        | 11.0  | 5885 | 0.5959          | 0.0611               |
| 0.5727        | 12.0  | 6420 | 0.6199          | 0.0303               |
| 0.556         | 13.0  | 6955 | 0.5929          | 0.0882               |
| 0.5635        | 14.0  | 7490 | 0.6288          | 0.0686               |
| 0.5531        | 15.0  | 8025 | 0.5977          | 0.0853               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
