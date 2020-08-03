# CasRel-pytorch-reimplement
Pytorch reimplement of the paper "A Novel Cascade Binary Tagging Framework for Relational Triple Extraction" ACL2020. The [original code](https://github.com/weizhepei/CasRel) was written in keras.
# Requirements
- keras-bert
- tensorflow-gpu
- transformers
# Dataset
- [CMED](biendata.xyz/competition/chip_2020_2/): CHIP-2020 中文医学文本实体关系抽取
# Usage
1. Get the pre-trained Chinese BERT model
   1. Download the vocab.txt of [BERT-wwm](https://github.com/ymcui/Chinese-BERT-wwm)
   2. Get the pre-trained BERT cache
   ```
   from transformers import *
   model = BertModel.from_pretrained("hfl/chinese-bert-wwm")
   ```
   p.s. I choose to use the chinese-bert-wwm here. You can also choose other pre-trained models like this.
