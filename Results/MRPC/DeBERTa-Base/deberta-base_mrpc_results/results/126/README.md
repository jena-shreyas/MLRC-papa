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
      value: 0.7745098039215687
    - name: F1
      type: f1
      value: 0.8466666666666667
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# output

This model is a fine-tuned version of [microsoft/deberta-base](https://huggingface.co/microsoft/deberta-base) on the GLUE MRPC dataset.
It achieves the following results on the evaluation set:
- Loss: 0.5059
- Accuracy: 0.7745
- F1: 0.8467
- Combined Score: 0.8106

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
| No log        | 1.0   | 230  | 0.5209          | 0.7451   | 0.8400 | 0.7925         |
| No log        | 2.0   | 460  | 0.5641          | 0.7353   | 0.8359 | 0.7856         |
| 0.5331        | 3.0   | 690  | 0.5156          | 0.7549   | 0.8452 | 0.8001         |
| 0.5331        | 4.0   | 920  | 0.5576          | 0.7377   | 0.8371 | 0.7874         |
| 0.4856        | 5.0   | 1150 | 0.5600          | 0.7426   | 0.8387 | 0.7907         |
| 0.4856        | 6.0   | 1380 | 0.4858          | 0.7843   | 0.8576 | 0.8210         |
| 0.4511        | 7.0   | 1610 | 0.5188          | 0.7819   | 0.8585 | 0.8202         |
| 0.4511        | 8.0   | 1840 | 0.5412          | 0.7696   | 0.8522 | 0.8109         |
| 0.4402        | 9.0   | 2070 | 0.5153          | 0.7745   | 0.8535 | 0.8140         |
| 0.4402        | 10.0  | 2300 | 0.5010          | 0.7647   | 0.8447 | 0.8047         |
| 0.4086        | 11.0  | 2530 | 0.5391          | 0.7721   | 0.8526 | 0.8123         |
| 0.4086        | 12.0  | 2760 | 0.5729          | 0.7475   | 0.8403 | 0.7939         |
| 0.4086        | 13.0  | 2990 | 0.5104          | 0.7794   | 0.8529 | 0.8162         |
| 0.3977        | 14.0  | 3220 | 0.4979          | 0.7843   | 0.8508 | 0.8176         |
| 0.3977        | 15.0  | 3450 | 0.5059          | 0.7745   | 0.8467 | 0.8106         |


### Framework versions

- Transformers 4.18.0
- Pytorch 1.8.2
- Datasets 2.8.0
- Tokenizers 0.12.1
