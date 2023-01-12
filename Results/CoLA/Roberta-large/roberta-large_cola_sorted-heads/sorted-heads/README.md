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
      value: 0.46612183496010656
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sorted-heads

This model is a fine-tuned version of [roberta-large](https://huggingface.co/roberta-large) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5122
- Matthews Correlation: 0.4661

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
- train_batch_size: 32
- eval_batch_size: 32
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: constant
- num_epochs: 15.0

### Training results

| Training Loss | Epoch | Step | Validation Loss | Matthews Correlation |
|:-------------:|:-----:|:----:|:---------------:|:--------------------:|
| No log        | 1.0   | 268  | 0.5854          | 0.1763               |
| 0.5161        | 2.0   | 536  | 0.5653          | 0.2929               |
| 0.5161        | 3.0   | 804  | 0.5388          | 0.3434               |
| 0.4564        | 4.0   | 1072 | 0.4983          | 0.3991               |
| 0.4564        | 5.0   | 1340 | 0.5379          | 0.3538               |
| 0.4364        | 6.0   | 1608 | 0.5445          | 0.4050               |
| 0.4364        | 7.0   | 1876 | 0.5162          | 0.4069               |
| 0.4143        | 8.0   | 2144 | 0.5345          | 0.3959               |
| 0.4143        | 9.0   | 2412 | 0.4827          | 0.4630               |
| 0.3985        | 10.0  | 2680 | 0.4867          | 0.4573               |
| 0.3985        | 11.0  | 2948 | 0.4424          | 0.5078               |
| 0.3875        | 12.0  | 3216 | 0.5083          | 0.4685               |
| 0.3875        | 13.0  | 3484 | 0.4688          | 0.4974               |
| 0.3759        | 14.0  | 3752 | 0.5506          | 0.4087               |
| 0.3639        | 15.0  | 4020 | 0.5122          | 0.4661               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
