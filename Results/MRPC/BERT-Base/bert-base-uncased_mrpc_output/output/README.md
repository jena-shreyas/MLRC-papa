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
      value: 0.7107843137254902
    - name: F1
      type: f1
      value: 0.8059210526315789
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.6353
- Accuracy: 0.7108
- F1: 0.8059
- Combined Score: 0.7584

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
| No log        | 1.0   | 230  | 0.5897          | 0.6912   | 0.8085 | 0.7498         |
| No log        | 2.0   | 460  | 0.6038          | 0.6961   | 0.8149 | 0.7555         |
| 0.5875        | 3.0   | 690  | 0.5933          | 0.7059   | 0.8142 | 0.7601         |
| 0.5875        | 4.0   | 920  | 0.5980          | 0.6961   | 0.8104 | 0.7532         |
| 0.555         | 5.0   | 1150 | 0.6031          | 0.7083   | 0.8161 | 0.7622         |
| 0.555         | 6.0   | 1380 | 0.5941          | 0.7157   | 0.8182 | 0.7669         |
| 0.5261        | 7.0   | 1610 | 0.6069          | 0.6985   | 0.8081 | 0.7533         |
| 0.5261        | 8.0   | 1840 | 0.6198          | 0.7157   | 0.8182 | 0.7669         |
| 0.5173        | 9.0   | 2070 | 0.6161          | 0.6912   | 0.7968 | 0.7440         |
| 0.5173        | 10.0  | 2300 | 0.6166          | 0.6863   | 0.7852 | 0.7358         |
| 0.4942        | 11.0  | 2530 | 0.6149          | 0.6985   | 0.7993 | 0.7489         |
| 0.4942        | 12.0  | 2760 | 0.6164          | 0.7034   | 0.8045 | 0.7540         |
| 0.4942        | 13.0  | 2990 | 0.6232          | 0.7010   | 0.7932 | 0.7471         |
| 0.483         | 14.0  | 3220 | 0.6412          | 0.6765   | 0.7643 | 0.7204         |
| 0.483         | 15.0  | 3450 | 0.6353          | 0.7108   | 0.8059 | 0.7584         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
