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
- name: sorted-heads
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
      value: 0.7647058823529411
    - name: F1
      type: f1
      value: 0.8415841584158414
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sorted-heads

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5498
- Accuracy: 0.7647
- F1: 0.8416
- Combined Score: 0.8031

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
| No log        | 1.0   | 230  | 0.5457          | 0.7279   | 0.8305 | 0.7792         |
| No log        | 2.0   | 460  | 0.5693          | 0.7353   | 0.8364 | 0.7858         |
| 0.538         | 3.0   | 690  | 0.5335          | 0.7475   | 0.8373 | 0.7924         |
| 0.538         | 4.0   | 920  | 0.5595          | 0.7426   | 0.8377 | 0.7902         |
| 0.4762        | 5.0   | 1150 | 0.5483          | 0.7475   | 0.8373 | 0.7924         |
| 0.4762        | 6.0   | 1380 | 0.5316          | 0.7574   | 0.8421 | 0.7997         |
| 0.4393        | 7.0   | 1610 | 0.5616          | 0.7574   | 0.8436 | 0.8005         |
| 0.4393        | 8.0   | 1840 | 0.5888          | 0.7525   | 0.8419 | 0.7972         |
| 0.4236        | 9.0   | 2070 | 0.5359          | 0.7647   | 0.8442 | 0.8044         |
| 0.4236        | 10.0  | 2300 | 0.5323          | 0.7721   | 0.8453 | 0.8087         |
| 0.3896        | 11.0  | 2530 | 0.5659          | 0.7647   | 0.8462 | 0.8054         |
| 0.3896        | 12.0  | 2760 | 0.6494          | 0.7525   | 0.8449 | 0.7987         |
| 0.3896        | 13.0  | 2990 | 0.5611          | 0.7745   | 0.8502 | 0.8123         |
| 0.3691        | 14.0  | 3220 | 0.5341          | 0.7794   | 0.8448 | 0.8121         |
| 0.3691        | 15.0  | 3450 | 0.5498          | 0.7647   | 0.8416 | 0.8031         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
