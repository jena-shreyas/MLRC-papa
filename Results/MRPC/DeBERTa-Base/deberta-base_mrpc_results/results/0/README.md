---
language:
- en
license: mit
tags:
- generated_from_trainer
datasets:
- glue
metrics:
- accuracy
- f1
model-index:
- name: output
  results:
  - task:
      name: Text Classification
      type: text-classification
    dataset:
      name: GLUE MRPC
      type: glue
      args: mrpc
    metrics:
    - name: Accuracy
      type: accuracy
      value: 0.7794117647058824
    - name: F1
      type: f1
      value: 0.8538961038961038
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5188
- Accuracy: 0.7794
- F1: 0.8539
- Combined Score: 0.8167

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

| Training Loss | Epoch | Step | Validation Loss | Accuracy | F1     | Combined Score |
|:-------------:|:-----:|:----:|:---------------:|:--------:|:------:|:--------------:|
| No log        | 1.0   | 230  | 0.5344          | 0.7525   | 0.8444 | 0.7984         |
| No log        | 2.0   | 460  | 0.5667          | 0.7402   | 0.8399 | 0.7900         |
| 0.5236        | 3.0   | 690  | 0.5207          | 0.7623   | 0.8487 | 0.8055         |
| 0.5236        | 4.0   | 920  | 0.5343          | 0.7598   | 0.8483 | 0.8041         |
| 0.4613        | 5.0   | 1150 | 0.5324          | 0.7475   | 0.8393 | 0.7934         |
| 0.4613        | 6.0   | 1380 | 0.4870          | 0.7819   | 0.8576 | 0.8197         |
| 0.4205        | 7.0   | 1610 | 0.5228          | 0.7647   | 0.8495 | 0.8071         |
| 0.4205        | 8.0   | 1840 | 0.5478          | 0.7647   | 0.8495 | 0.8071         |
| 0.4034        | 9.0   | 2070 | 0.5005          | 0.7843   | 0.8581 | 0.8212         |
| 0.4034        | 10.0  | 2300 | 0.4939          | 0.7892   | 0.8571 | 0.8232         |
| 0.3695        | 11.0  | 2530 | 0.5140          | 0.7819   | 0.8558 | 0.8188         |
| 0.3695        | 12.0  | 2760 | 0.6217          | 0.7574   | 0.8484 | 0.8029         |
| 0.3695        | 13.0  | 2990 | 0.5246          | 0.7721   | 0.8502 | 0.8112         |
| 0.3508        | 14.0  | 3220 | 0.4829          | 0.7721   | 0.8410 | 0.8065         |
| 0.3508        | 15.0  | 3450 | 0.5188          | 0.7794   | 0.8539 | 0.8167         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
