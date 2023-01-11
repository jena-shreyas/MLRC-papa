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
      value: 0.7573529411764706
    - name: F1
      type: f1
      value: 0.8426073131955484
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5896
- Accuracy: 0.7574
- F1: 0.8426
- Combined Score: 0.8000

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
| No log        | 1.0   | 230  | 0.5569          | 0.7108   | 0.8196 | 0.7652         |
| No log        | 2.0   | 460  | 0.5772          | 0.7181   | 0.8265 | 0.7723         |
| 0.5479        | 3.0   | 690  | 0.5528          | 0.7304   | 0.8297 | 0.7801         |
| 0.5479        | 4.0   | 920  | 0.5866          | 0.7328   | 0.8351 | 0.7840         |
| 0.4981        | 5.0   | 1150 | 0.5850          | 0.7304   | 0.8302 | 0.7803         |
| 0.4981        | 6.0   | 1380 | 0.5602          | 0.75     | 0.8416 | 0.7958         |
| 0.4645        | 7.0   | 1610 | 0.5798          | 0.75     | 0.8426 | 0.7963         |
| 0.4645        | 8.0   | 1840 | 0.5912          | 0.7525   | 0.8414 | 0.7969         |
| 0.4454        | 9.0   | 2070 | 0.5538          | 0.7426   | 0.8309 | 0.7868         |
| 0.4454        | 10.0  | 2300 | 0.5616          | 0.7574   | 0.8411 | 0.7992         |
| 0.4195        | 11.0  | 2530 | 0.5821          | 0.7426   | 0.8341 | 0.7884         |
| 0.4195        | 12.0  | 2760 | 0.6299          | 0.7475   | 0.8423 | 0.7949         |
| 0.4195        | 13.0  | 2990 | 0.5941          | 0.7451   | 0.8344 | 0.7897         |
| 0.4016        | 14.0  | 3220 | 0.5695          | 0.7475   | 0.8292 | 0.7884         |
| 0.4016        | 15.0  | 3450 | 0.5896          | 0.7574   | 0.8426 | 0.8000         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
