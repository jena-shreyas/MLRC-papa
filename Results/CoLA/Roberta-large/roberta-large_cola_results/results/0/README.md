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
- name: output
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
      value: 0.5159673470694772
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [roberta-large](https://huggingface.co/roberta-large) on the GLUE COLA dataset.
It achieves the following results on the evaluation set:
- Loss: 0.4724
- Matthews Correlation: 0.5160

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
| No log        | 1.0   | 268  | 0.5519          | 0.3048               |
| 0.488         | 2.0   | 536  | 0.5532          | 0.3655               |
| 0.488         | 3.0   | 804  | 0.5146          | 0.3845               |
| 0.4218        | 4.0   | 1072 | 0.4711          | 0.4741               |
| 0.4218        | 5.0   | 1340 | 0.5345          | 0.4009               |
| 0.4079        | 6.0   | 1608 | 0.5191          | 0.4443               |
| 0.4079        | 7.0   | 1876 | 0.5095          | 0.4553               |
| 0.3882        | 8.0   | 2144 | 0.5153          | 0.4562               |
| 0.3882        | 9.0   | 2412 | 0.4738          | 0.4790               |
| 0.3697        | 10.0  | 2680 | 0.4810          | 0.4906               |
| 0.3697        | 11.0  | 2948 | 0.4227          | 0.5547               |
| 0.3646        | 12.0  | 3216 | 0.5159          | 0.4900               |
| 0.3646        | 13.0  | 3484 | 0.4455          | 0.5317               |
| 0.3501        | 14.0  | 3752 | 0.5474          | 0.4822               |
| 0.3377        | 15.0  | 4020 | 0.4724          | 0.5160               |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
