# SSD、YOLO用 データセット生成ツール

## 概要
SSDお勉強用のデータセット作成と、ChainerCVを用いた学習セット一式です

## 環境

Python 3.x
Chainer 4.4
ChainerCV 0.10

## 使い方

### データ生成

* coin_dataset.ipynb ... 画像を生成する Jupyter Notebook です
* japanese_coin/coin ... 検出対象となる画像を格納します。透過pngがおすすめ
* japanese_coin/tex ... 背景となる画像を格納します。

### 学習

* ssd_train-coin.ipynb ... 生成した画像セットで学習を行います。内容はChainerCVのSSD学習サンプルと同じです。
