---
license: other
library_name: peft
tags:
- llama-factory
- lora
- generated_from_trainer
base_model: /mnt/workspace/yangjingtao/reward_model/Qwen1.5-7B
model-index:
- name: sft-citation
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft-citation

This model is a fine-tuned version of [/mnt/workspace/yangjingtao/reward_model/Qwen1.5-7B](https://huggingface.co//mnt/workspace/yangjingtao/reward_model/Qwen1.5-7B) on the citation_train dataset.
It achieves the following results on the evaluation set:
- Loss: 1.8063

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 1
- eval_batch_size: 1
- seed: 42
- gradient_accumulation_steps: 8
- total_train_batch_size: 8
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_steps: 0.1
- num_epochs: 3.0
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step  | Validation Loss |
|:-------------:|:-----:|:-----:|:---------------:|
| 1.839         | 0.05  | 500   | 1.9732          |
| 1.8557        | 0.1   | 1000  | 1.9410          |
| 1.9781        | 0.16  | 1500  | 1.9233          |
| 1.8874        | 0.21  | 2000  | 1.9129          |
| 1.9058        | 0.26  | 2500  | 1.9056          |
| 1.8286        | 0.31  | 3000  | 1.8981          |
| 1.8911        | 0.36  | 3500  | 1.8920          |
| 1.9629        | 0.42  | 4000  | 1.8872          |
| 1.8378        | 0.47  | 4500  | 1.8792          |
| 1.8603        | 0.52  | 5000  | 1.8738          |
| 1.7926        | 0.57  | 5500  | 1.8695          |
| 1.9403        | 0.62  | 6000  | 1.8636          |
| 1.779         | 0.67  | 6500  | 1.8612          |
| 1.9105        | 0.73  | 7000  | 1.8564          |
| 1.7674        | 0.78  | 7500  | 1.8519          |
| 1.8626        | 0.83  | 8000  | 1.8503          |
| 1.8678        | 0.88  | 8500  | 1.8455          |
| 1.9112        | 0.93  | 9000  | 1.8427          |
| 1.9299        | 0.99  | 9500  | 1.8397          |
| 1.7281        | 1.04  | 10000 | 1.8387          |
| 1.7473        | 1.09  | 10500 | 1.8369          |
| 1.8333        | 1.14  | 11000 | 1.8355          |
| 1.8227        | 1.19  | 11500 | 1.8335          |
| 1.7638        | 1.25  | 12000 | 1.8308          |
| 1.8019        | 1.3   | 12500 | 1.8287          |
| 1.758         | 1.35  | 13000 | 1.8267          |
| 1.6836        | 1.4   | 13500 | 1.8257          |
| 1.6567        | 1.45  | 14000 | 1.8220          |
| 1.7226        | 1.5   | 14500 | 1.8212          |
| 1.7041        | 1.56  | 15000 | 1.8174          |
| 1.8078        | 1.61  | 15500 | 1.8171          |
| 1.7383        | 1.66  | 16000 | 1.8166          |
| 1.8053        | 1.71  | 16500 | 1.8131          |
| 1.8089        | 1.76  | 17000 | 1.8104          |
| 1.8332        | 1.82  | 17500 | 1.8092          |
| 1.8147        | 1.87  | 18000 | 1.8086          |
| 1.6932        | 1.92  | 18500 | 1.8060          |
| 1.7515        | 1.97  | 19000 | 1.8047          |
| 1.5257        | 2.02  | 19500 | 1.8105          |
| 1.6507        | 2.08  | 20000 | 1.8111          |
| 1.6245        | 2.13  | 20500 | 1.8106          |
| 1.6069        | 2.18  | 21000 | 1.8109          |
| 1.6378        | 2.23  | 21500 | 1.8107          |
| 1.6624        | 2.28  | 22000 | 1.8101          |
| 1.6366        | 2.34  | 22500 | 1.8092          |
| 1.5974        | 2.39  | 23000 | 1.8095          |
| 1.6343        | 2.44  | 23500 | 1.8081          |
| 1.6166        | 2.49  | 24000 | 1.8084          |
| 1.7609        | 2.54  | 24500 | 1.8081          |
| 1.5347        | 2.59  | 25000 | 1.8076          |
| 1.6027        | 2.65  | 25500 | 1.8072          |
| 1.7376        | 2.7   | 26000 | 1.8066          |
| 1.7109        | 2.75  | 26500 | 1.8065          |
| 1.7087        | 2.8   | 27000 | 1.8064          |
| 1.655         | 2.85  | 27500 | 1.8064          |
| 1.7042        | 2.91  | 28000 | 1.8063          |
| 1.5426        | 2.96  | 28500 | 1.8063          |


### Framework versions

- PEFT 0.10.0
- Transformers 4.38.2
- Pytorch 2.1.2+cu121
- Datasets 2.16.1
- Tokenizers 0.15.1