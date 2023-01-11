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
      value: 0.7573529411764706
    - name: F1
      type: f1
      value: 0.8347245409015026
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5241
- Accuracy: 0.7574
- F1: 0.8347
- Combined Score: 0.7960

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
| No log        | 1.0   | 230  | 0.5361          | 0.7328   | 0.8320 | 0.7824         |
| No log        | 2.0   | 460  | 0.5819          | 0.7328   | 0.8346 | 0.7837         |
| 0.5342        | 3.0   | 690  | 0.5406          | 0.7475   | 0.8403 | 0.7939         |
| 0.5342        | 4.0   | 920  | 0.5730          | 0.7304   | 0.8323 | 0.7814         |
| 0.4847        | 5.0   | 1150 | 0.5568          | 0.7549   | 0.8442 | 0.7996         |
| 0.4847        | 6.0   | 1380 | 0.5162          | 0.7794   | 0.8562 | 0.8178         |
| 0.4539        | 7.0   | 1610 | 0.5342          | 0.7696   | 0.8517 | 0.8107         |
| 0.4539        | 8.0   | 1840 | 0.5662          | 0.7647   | 0.8491 | 0.8069         |
| 0.4431        | 9.0   | 2070 | 0.5361          | 0.7672   | 0.848  | 0.8076         |
| 0.4431        | 10.0  | 2300 | 0.5180          | 0.7696   | 0.8439 | 0.8067         |
| 0.4128        | 11.0  | 2530 | 0.5542          | 0.7525   | 0.8399 | 0.7962         |
| 0.4128        | 12.0  | 2760 | 0.6065          | 0.7525   | 0.8444 | 0.7984         |
| 0.4128        | 13.0  | 2990 | 0.5396          | 0.7672   | 0.8455 | 0.8063         |
| 0.3982        | 14.0  | 3220 | 0.5223          | 0.7475   | 0.8221 | 0.7848         |
| 0.3982        | 15.0  | 3450 | 0.5241          | 0.7574   | 0.8347 | 0.7960         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
