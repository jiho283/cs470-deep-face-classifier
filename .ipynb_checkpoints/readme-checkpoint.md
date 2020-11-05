# CS470 Project

# Crawling

Install google-images-download library

pip install git+http://github.com/Joeclinton1/google-images-download.git

강아지상 : 워너원 강다니엘, 엑소 백현, 박보검,송중기, 임시완, 박보영, 손예진, 태연, 아이유, 한효주

고양이상 : 워너원 황민현, 엑소 시우민, 강동원, 이종석, 이준기, 한예슬,유인영,김희선,이나영,한채영

곰상 : 마동석, 조진웅, 조세호, 안재홍, 정형돈, 스윙스, 박성웅, 최자, 곽도원, 김구라

공룡상 : 윤두준, 이민기, 김우빈, 육성재, 공유, 송지효, 김아중, 한지민, 천우희, 신민아

토끼상 : 방탄소년단 정국, 아이콘 바비, 워너원 박지훈, 엑소 수호, 안형섭, 수지, 트와이스 나연, 트와이스 다현, 이세영, 백진희

대머리상 : from kaggle

# Dataset download
```
$ wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=1W5HKr-M1J98smLiF781jjiLVxl9hmq0i' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=1W5HKr-M1J98smLiF781jjiLVxl9hmq0i" -O animal.zip && rm -rf /tmp/cookies.txt

$ wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=1yUAutv-VWkfUm1rvbzXcmtOaASvS3dwR' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=1yUAutv-VWkfUm1rvbzXcmtOaASvS3dwR" -O bald.zip && rm -rf /tmp/cookies.txt
```

# Directory structure

# Quick Start
```

$ python3 train.py --exp_name baseline --coeff 0 --learning_rate 4e-3 --batch_size 128 --n_epoch 100 --optim adamw --weight_decay 1e-5 --num_workers 16 --warmup 1 --mixup_prob 1 --mixup_alpha 1 --label_smoothing 0.05  

$

```