---
language:
- en
license: apache-2.0
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
      value: 0.7524509803921569
    - name: F1
      type: f1
      value: 0.8373590982286634
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5739
- Accuracy: 0.7525
- F1: 0.8374
- Combined Score: 0.7949

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
| No log        | 1.0   | 230  | 0.5432          | 0.7108   | 0.8179 | 0.7643         |
| No log        | 2.0   | 460  | 0.5621          | 0.7230   | 0.8275 | 0.7753         |
| 0.5401        | 3.0   | 690  | 0.5388          | 0.7451   | 0.8370 | 0.7910         |
| 0.5401        | 4.0   | 920  | 0.5727          | 0.7402   | 0.8384 | 0.7893         |
| 0.4903        | 5.0   | 1150 | 0.5727          | 0.7377   | 0.8336 | 0.7857         |
| 0.4903        | 6.0   | 1380 | 0.5440          | 0.7451   | 0.8360 | 0.7905         |
| 0.4567        | 7.0   | 1610 | 0.5558          | 0.7525   | 0.8399 | 0.7962         |
| 0.4567        | 8.0   | 1840 | 0.5821          | 0.7451   | 0.8370 | 0.7910         |
| 0.4413        | 9.0   | 2070 | 0.5497          | 0.7451   | 0.8323 | 0.7887         |
| 0.4413        | 10.0  | 2300 | 0.5467          | 0.7426   | 0.8276 | 0.7851         |
| 0.4112        | 11.0  | 2530 | 0.5754          | 0.7598   | 0.8449 | 0.8024         |
| 0.4112        | 12.0  | 2760 | 0.6157          | 0.7525   | 0.8439 | 0.7982         |
| 0.4112        | 13.0  | 2990 | 0.5760          | 0.7525   | 0.8368 | 0.7946         |
| 0.3989        | 14.0  | 3220 | 0.5579          | 0.7353   | 0.8157 | 0.7755         |
| 0.3989        | 15.0  | 3450 | 0.5739          | 0.7525   | 0.8374 | 0.7949         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
