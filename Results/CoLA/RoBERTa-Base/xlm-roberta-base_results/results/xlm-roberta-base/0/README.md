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
      value: 0.31236083623809213
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5566
- Matthews Correlation: 0.3124

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
| 0.6008        | 1.0   | 535  | 0.6156          | 0.0                  |
| 0.5761        | 2.0   | 1070 | 0.5922          | 0.0656               |
| 0.5688        | 3.0   | 1605 | 0.5978          | 0.0722               |
| 0.5501        | 4.0   | 2140 | 0.5756          | 0.1418               |
| 0.5557        | 5.0   | 2675 | 0.5669          | 0.1929               |
| 0.5469        | 6.0   | 3210 | 0.5835          | 0.1647               |
| 0.5415        | 7.0   | 3745 | 0.5905          | 0.1706               |
| 0.5268        | 8.0   | 4280 | 0.5926          | 0.1929               |
| 0.5341        | 9.0   | 4815 | 0.5687          | 0.2459               |
| 0.5222        | 10.0  | 5350 | 0.5809          | 0.2474               |
| 0.5171        | 11.0  | 5885 | 0.5706          | 0.2875               |
| 0.5299        | 12.0  | 6420 | 0.5861          | 0.2474               |
| 0.5077        | 13.0  | 6955 | 0.5652          | 0.3107               |
| 0.5162        | 14.0  | 7490 | 0.6001          | 0.2431               |
| 0.5044        | 15.0  | 8025 | 0.5566          | 0.3124               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
