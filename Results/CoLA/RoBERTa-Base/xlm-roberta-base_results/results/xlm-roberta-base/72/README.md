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
      value: 0.2366138017243775
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5672
- Matthews Correlation: 0.2366

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
| 0.6018        | 1.0   | 535  | 0.6169          | 0.0                  |
| 0.5787        | 2.0   | 1070 | 0.5979          | -0.0207              |
| 0.5748        | 3.0   | 1605 | 0.6038          | 0.0029               |
| 0.5588        | 4.0   | 2140 | 0.5869          | 0.0723               |
| 0.5632        | 5.0   | 2675 | 0.5782          | 0.1487               |
| 0.5562        | 6.0   | 3210 | 0.5948          | 0.1107               |
| 0.5493        | 7.0   | 3745 | 0.6075          | 0.1434               |
| 0.5395        | 8.0   | 4280 | 0.6021          | 0.1682               |
| 0.5454        | 9.0   | 4815 | 0.5829          | 0.1812               |
| 0.5372        | 10.0  | 5350 | 0.5919          | 0.1636               |
| 0.5259        | 11.0  | 5885 | 0.5797          | 0.2234               |
| 0.5418        | 12.0  | 6420 | 0.5960          | 0.2059               |
| 0.519         | 13.0  | 6955 | 0.5798          | 0.2399               |
| 0.5255        | 14.0  | 7490 | 0.6010          | 0.2102               |
| 0.52          | 15.0  | 8025 | 0.5672          | 0.2366               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
