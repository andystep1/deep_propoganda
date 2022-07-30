Text can be parsed from telegram channels with https://github.com/bellingcat/snscrape
```
snscrape --jsonl telegram-channel __username__ > __filename__.json;
```
text_preparation.ipynb reads multiple jsons, removes links, hashtags, usertags and emoji, and saves parsed channels as plain text file.

Use this file in train_and_save.ipynb to train model and save weights.

load_and_generate.ipynb uses previously saved weights to generate text

have fun
