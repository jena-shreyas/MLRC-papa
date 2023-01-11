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
      value: 0.12272769082044643
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5895
- Matthews Correlation: 0.1227

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
| 0.6077        | 1.0   | 535  | 0.6146          | 0.0                  |
| 0.593         | 2.0   | 1070 | 0.6039          | 0.0                  |
| 0.5932        | 3.0   | 1605 | 0.6083          | 0.0                  |
| 0.5819        | 4.0   | 2140 | 0.5915          | 0.0593               |
| 0.5852        | 5.0   | 2675 | 0.5905          | 0.0762               |
| 0.5799        | 6.0   | 3210 | 0.6101          | 0.0315               |
| 0.5748        | 7.0   | 3745 | 0.6085          | 0.0602               |
| 0.5688        | 8.0   | 4280 | 0.6111          | 0.0620               |
| 0.5718        | 9.0   | 4815 | 0.5941          | 0.0786               |
| 0.5653        | 10.0  | 5350 | 0.6039          | 0.0664               |
| 0.5561        | 11.0  | 5885 | 0.5904          | 0.1135               |
| 0.5682        | 12.0  | 6420 | 0.6184          | 0.0642               |
| 0.5495        | 13.0  | 6955 | 0.5859          | 0.1302               |
| 0.558         | 14.0  | 7490 | 0.6200          | 0.0797               |
| 0.5473        | 15.0  | 8025 | 0.5895          | 0.1227               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
