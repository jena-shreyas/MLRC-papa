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
      value: 0.7303921568627451
    - name: F1
      type: f1
      value: 0.8202614379084968
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5851
- Accuracy: 0.7304
- F1: 0.8203
- Combined Score: 0.7753

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
| No log        | 1.0   | 230  | 0.5564          | 0.7132   | 0.8208 | 0.7670         |
| No log        | 2.0   | 460  | 0.5791          | 0.7206   | 0.8278 | 0.7742         |
| 0.557         | 3.0   | 690  | 0.5563          | 0.7304   | 0.8287 | 0.7795         |
| 0.557         | 4.0   | 920  | 0.5777          | 0.7304   | 0.8318 | 0.7811         |
| 0.5166        | 5.0   | 1150 | 0.5781          | 0.7279   | 0.8279 | 0.7779         |
| 0.5166        | 6.0   | 1380 | 0.5562          | 0.7426   | 0.8346 | 0.7886         |
| 0.4816        | 7.0   | 1610 | 0.5661          | 0.7377   | 0.8310 | 0.7844         |
| 0.4816        | 8.0   | 1840 | 0.5839          | 0.7353   | 0.8286 | 0.7819         |
| 0.4721        | 9.0   | 2070 | 0.5712          | 0.7279   | 0.8213 | 0.7746         |
| 0.4721        | 10.0  | 2300 | 0.5679          | 0.7328   | 0.8216 | 0.7772         |
| 0.447         | 11.0  | 2530 | 0.5864          | 0.7255   | 0.8199 | 0.7727         |
| 0.447         | 12.0  | 2760 | 0.6111          | 0.7402   | 0.8359 | 0.7881         |
| 0.447         | 13.0  | 2990 | 0.5819          | 0.7328   | 0.8204 | 0.7766         |
| 0.4354        | 14.0  | 3220 | 0.5817          | 0.7230   | 0.8094 | 0.7662         |
| 0.4354        | 15.0  | 3450 | 0.5851          | 0.7304   | 0.8203 | 0.7753         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
