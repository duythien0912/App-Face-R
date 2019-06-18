<h1 align="center">Welcome to face-recognition 👋</h1>
<p>
  <img src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
</p>

> Face recognition

## Required

Add 2 folder
```sh
dataset/*

videos/*
```

## Create data from video

```sh
python3 gather_examples.py --input videos/quan.m4v --output dataset/quan --detector face_detector --skip 6 --name quan
```

## Install

```sh
pip install requirements.txt
```

## Train

```sh
python3 train.py --dataset dataset --model thien.model --labelbin lb.pickle
```

## Convert Model to to CoreML

```sh
python3 coremlconverter.py --model thien.model --labelbin lb.pickle
```
<!-- 
## Run tests

```sh
python test
``` -->

## Author

👤 **duythien**

* Github: [@duythien0912](https://github.com/duythien0912)

## Show your support

Give a ⭐️ if this project helped you !

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_