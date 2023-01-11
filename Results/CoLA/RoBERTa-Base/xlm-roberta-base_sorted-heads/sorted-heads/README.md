---
language:
- en
license: mit
tags:
- generated_from_trainer
datasets:
- glue
metrics:
- matthews_correlation
model-index:
- name: sorted-heads
  results:
  - task:
      name: Text Classification
      type: text-classification
    dataset:
      name: GLUE COLA
      type: glue
      args: cola
    metrics:
    - name: Matthews Correlation
      type: matthews_correlation
      value: 0.2676743198156292
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sorted-heads

This model is a fine-tuned version of [xlm-roberta-base](https://huggingface.co/xlm-roberta-base) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5621
- Matthews Correlation: 0.2677

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

| Training Loss | Epoch | Step | Validation Loss | Matthews Correlation |
|:-------------:|:-----:|:----:|:---------------:|:--------------------:|
| 0.6017        | 1.0   | 535  | 0.6162          | 0.0                  |
| 0.579         | 2.0   | 1070 | 0.5938          | 0.0181               |
| 0.5735        | 3.0   | 1605 | 0.6001          | 0.0840               |
| 0.5586        | 4.0   | 2140 | 0.5800          | 0.1285               |
| 0.5622        | 5.0   | 2675 | 0.5752          | 0.1519               |
| 0.554         | 6.0   | 3210 | 0.5910          | 0.1487               |
| 0.5485        | 7.0   | 3745 | 0.5980          | 0.1667               |
| 0.5356        | 8.0   | 4280 | 0.5962          | 0.1773               |
| 0.5414        | 9.0   | 4815 | 0.5717          | 0.2003               |
| 0.5326        | 10.0  | 5350 | 0.5862          | 0.2045               |
| 0.524         | 11.0  | 5885 | 0.5718          | 0.2312               |
| 0.5384        | 12.0  | 6420 | 0.5894          | 0.2139               |
| 0.515         | 13.0  | 6955 | 0.5655          | 0.2424               |
| 0.5227        | 14.0  | 7490 | 0.5937          | 0.2046               |
| 0.5124        | 15.0  | 8025 | 0.5621          | 0.2677               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
