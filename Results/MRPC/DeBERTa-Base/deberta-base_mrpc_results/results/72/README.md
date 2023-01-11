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
      value: 0.7941176470588235
    - name: F1
      type: f1
      value: 0.8631921824104234
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.4617
- Accuracy: 0.7941
- F1: 0.8632
- Combined Score: 0.8287

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
| No log        | 1.0   | 230  | 0.5013          | 0.7623   | 0.8477 | 0.8050         |
| No log        | 2.0   | 460  | 0.5228          | 0.7794   | 0.8602 | 0.8198         |
| 0.5053        | 3.0   | 690  | 0.4864          | 0.7819   | 0.8603 | 0.8211         |
| 0.5053        | 4.0   | 920  | 0.5048          | 0.7721   | 0.8554 | 0.8137         |
| 0.4405        | 5.0   | 1150 | 0.4920          | 0.7794   | 0.8576 | 0.8185         |
| 0.4405        | 6.0   | 1380 | 0.4384          | 0.7990   | 0.8656 | 0.8323         |
| 0.4044        | 7.0   | 1610 | 0.4609          | 0.7941   | 0.8650 | 0.8295         |
| 0.4044        | 8.0   | 1840 | 0.5123          | 0.7917   | 0.8644 | 0.8281         |
| 0.3856        | 9.0   | 2070 | 0.4445          | 0.8039   | 0.8693 | 0.8366         |
| 0.3856        | 10.0  | 2300 | 0.4418          | 0.8113   | 0.8697 | 0.8405         |
| 0.3577        | 11.0  | 2530 | 0.4859          | 0.8088   | 0.8742 | 0.8415         |
| 0.3577        | 12.0  | 2760 | 0.5596          | 0.7794   | 0.8602 | 0.8198         |
| 0.3577        | 13.0  | 2990 | 0.4716          | 0.7941   | 0.8632 | 0.8287         |
| 0.3381        | 14.0  | 3220 | 0.4464          | 0.7966   | 0.8600 | 0.8283         |
| 0.3381        | 15.0  | 3450 | 0.4617          | 0.7941   | 0.8632 | 0.8287         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
