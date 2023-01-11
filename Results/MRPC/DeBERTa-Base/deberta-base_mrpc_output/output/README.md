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
      value: 0.6862745098039216
    - name: F1
      type: f1
      value: 0.7830508474576272
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.6307
- Accuracy: 0.6863
- F1: 0.7831
- Combined Score: 0.7347

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
| No log        | 1.0   | 230  | 0.5843          | 0.7010   | 0.8146 | 0.7578         |
| No log        | 2.0   | 460  | 0.6026          | 0.6961   | 0.8138 | 0.7549         |
| 0.587         | 3.0   | 690  | 0.5836          | 0.7083   | 0.8138 | 0.7611         |
| 0.587         | 4.0   | 920  | 0.5893          | 0.7034   | 0.8130 | 0.7582         |
| 0.5528        | 5.0   | 1150 | 0.5995          | 0.7181   | 0.8217 | 0.7699         |
| 0.5528        | 6.0   | 1380 | 0.5826          | 0.7157   | 0.8141 | 0.7649         |
| 0.5292        | 7.0   | 1610 | 0.5982          | 0.7157   | 0.8147 | 0.7652         |
| 0.5292        | 8.0   | 1840 | 0.6140          | 0.7230   | 0.8186 | 0.7708         |
| 0.514         | 9.0   | 2070 | 0.6121          | 0.7206   | 0.8185 | 0.7695         |
| 0.514         | 10.0  | 2300 | 0.6127          | 0.6838   | 0.7787 | 0.7313         |
| 0.4891        | 11.0  | 2530 | 0.6108          | 0.6887   | 0.7894 | 0.7391         |
| 0.4891        | 12.0  | 2760 | 0.6172          | 0.6838   | 0.7882 | 0.7360         |
| 0.4891        | 13.0  | 2990 | 0.6124          | 0.7010   | 0.7932 | 0.7471         |
| 0.4756        | 14.0  | 3220 | 0.6527          | 0.6716   | 0.7528 | 0.7122         |
| 0.4756        | 15.0  | 3450 | 0.6307          | 0.6863   | 0.7831 | 0.7347         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
