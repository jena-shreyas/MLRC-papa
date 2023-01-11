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
      value: 0.75
    - name: F1
      type: f1
      value: 0.8365384615384615
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sorted-heads

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5826
- Accuracy: 0.75
- F1: 0.8365
- Combined Score: 0.7933

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
| No log        | 1.0   | 230  | 0.5533          | 0.7132   | 0.8208 | 0.7670         |
| No log        | 2.0   | 460  | 0.5703          | 0.7279   | 0.8321 | 0.7800         |
| 0.5513        | 3.0   | 690  | 0.5463          | 0.7279   | 0.8274 | 0.7777         |
| 0.5513        | 4.0   | 920  | 0.5752          | 0.7353   | 0.8359 | 0.7856         |
| 0.5039        | 5.0   | 1150 | 0.5778          | 0.7328   | 0.8310 | 0.7819         |
| 0.5039        | 6.0   | 1380 | 0.5522          | 0.7402   | 0.8333 | 0.7868         |
| 0.4697        | 7.0   | 1610 | 0.5698          | 0.75     | 0.8411 | 0.7956         |
| 0.4697        | 8.0   | 1840 | 0.5890          | 0.7426   | 0.8346 | 0.7886         |
| 0.4555        | 9.0   | 2070 | 0.5571          | 0.7475   | 0.8341 | 0.7908         |
| 0.4555        | 10.0  | 2300 | 0.5590          | 0.7353   | 0.8235 | 0.7794         |
| 0.4272        | 11.0  | 2530 | 0.5749          | 0.7549   | 0.8408 | 0.7978         |
| 0.4272        | 12.0  | 2760 | 0.6129          | 0.7549   | 0.8457 | 0.8003         |
| 0.4272        | 13.0  | 2990 | 0.5879          | 0.75     | 0.8355 | 0.7927         |
| 0.4134        | 14.0  | 3220 | 0.5684          | 0.7328   | 0.8156 | 0.7742         |
| 0.4134        | 15.0  | 3450 | 0.5826          | 0.75     | 0.8365 | 0.7933         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
