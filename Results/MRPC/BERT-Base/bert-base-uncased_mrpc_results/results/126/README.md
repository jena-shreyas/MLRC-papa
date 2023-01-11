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
      value: 0.7230392156862745
    - name: F1
      type: f1
      value: 0.8168557536466775
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.6200
- Accuracy: 0.7230
- F1: 0.8169
- Combined Score: 0.7699

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
| No log        | 1.0   | 230  | 0.5888          | 0.7010   | 0.8163 | 0.7586         |
| No log        | 2.0   | 460  | 0.6037          | 0.7034   | 0.8191 | 0.7613         |
| 0.5823        | 3.0   | 690  | 0.5875          | 0.7157   | 0.8210 | 0.7683         |
| 0.5823        | 4.0   | 920  | 0.5898          | 0.7255   | 0.8293 | 0.7774         |
| 0.5459        | 5.0   | 1150 | 0.5965          | 0.7108   | 0.8162 | 0.7635         |
| 0.5459        | 6.0   | 1380 | 0.5839          | 0.7157   | 0.8187 | 0.7672         |
| 0.5152        | 7.0   | 1610 | 0.5913          | 0.7132   | 0.8169 | 0.7651         |
| 0.5152        | 8.0   | 1840 | 0.6123          | 0.7206   | 0.8213 | 0.7710         |
| 0.5023        | 9.0   | 2070 | 0.5976          | 0.7059   | 0.8052 | 0.7555         |
| 0.5023        | 10.0  | 2300 | 0.6007          | 0.7059   | 0.8026 | 0.7543         |
| 0.478         | 11.0  | 2530 | 0.6068          | 0.6985   | 0.8013 | 0.7499         |
| 0.478         | 12.0  | 2760 | 0.6146          | 0.7279   | 0.8263 | 0.7771         |
| 0.478         | 13.0  | 2990 | 0.6085          | 0.7083   | 0.8027 | 0.7555         |
| 0.4683        | 14.0  | 3220 | 0.6210          | 0.6936   | 0.7826 | 0.7381         |
| 0.4683        | 15.0  | 3450 | 0.6200          | 0.7230   | 0.8169 | 0.7699         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
