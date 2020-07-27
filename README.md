# toolkits for NLP

## intent
 为了方便自己学习与理解一些东西，实现一些自己的想法

## Update info:
  - <stong> 2020.7.27 </stong>strong> 完成 pretraining，用法参照 pretraining/README.md
  - <strong>2020.07.18</strong>  完成了tokenizer， 用法：
  ```python
from toolkit4nlp.tokenizers import Tokenizer
vocab = ''
tokenizer = Tokenizer(vocab, do_lower_case=True)
tokenizer.encode('我爱你中国')    
```
  - <strong>2020.07.16</strong>  完成bert加载预训练权重，用法：
  ```python
from toolkit4nlp.models import build_transformer_model

config_path = ''
checkpoints_path = ''
model = build_transformer_model(config_path, checkpoints_path)
  ```
  
  主要参考了<a href='https://github.com/google-research/bert.git'>bert</a> 和
  <a href='https://github.com/bojone/bert4keras.git'>bert4keras</a>以及
  <a href='https://github.com/CyberZHG/keras-bert'>keras_bert</a>
