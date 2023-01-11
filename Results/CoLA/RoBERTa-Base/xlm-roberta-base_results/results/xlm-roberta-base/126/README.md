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
      value: 0.17370331286638843
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5751
- Matthews Correlation: 0.1737

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
| 0.6059        | 1.0   | 535  | 0.6148          | 0.0                  |
| 0.5894        | 2.0   | 1070 | 0.6002          | 0.0                  |
| 0.5885        | 3.0   | 1605 | 0.6041          | 0.0656               |
| 0.5766        | 4.0   | 2140 | 0.5874          | 0.0467               |
| 0.5781        | 5.0   | 2675 | 0.5837          | 0.0797               |
| 0.5726        | 6.0   | 3210 | 0.6028          | 0.0498               |
| 0.5669        | 7.0   | 3745 | 0.6052          | 0.0836               |
| 0.5602        | 8.0   | 4280 | 0.6040          | 0.0762               |
| 0.5618        | 9.0   | 4815 | 0.5853          | 0.0890               |
| 0.5577        | 10.0  | 5350 | 0.5976          | 0.0763               |
| 0.5471        | 11.0  | 5885 | 0.5802          | 0.1350               |
| 0.5592        | 12.0  | 6420 | 0.6035          | 0.1394               |
| 0.5385        | 13.0  | 6955 | 0.5748          | 0.1548               |
| 0.5483        | 14.0  | 7490 | 0.6168          | 0.1124               |
| 0.5378        | 15.0  | 8025 | 0.5751          | 0.1737               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
