# SSD、YOLO等向け 学習データセット生成ツール

SSDお勉強用のデータセット作成と、ChainerCVを用いた学習セット一式です

![preview](https://user-images.githubusercontent.com/26473720/44628613-1e0de280-a97e-11e8-8dff-1a0349a1bec5.jpg)

## 環境

- Python 3.x
- Chainer 4.4
- ChainerCV 0.10

## ファイル

### データ生成

* coin_dataset.ipynb ... Jupyter Notebook 形式のスクリプトを進めると、以下のファイルを生成します
  * coin/JPEGImages **生成した画像**
  * coin/Annotations **画像に対応する領域情報のxml**
  * coin/ImageSets **train/valの振り分け情報**
* japanese_coin/coin ... 検出対象となる画像を格納します。透過pngがおすすめ。
  * ファイル名からラベル名を作ってるので、新たな画像を使う場合は気をつけてください。
* japanese_coin/tex ... 背景となる画像を格納します。

### 学習

* ssd_train-coin.ipynb ... 生成した画像セットで学習を行います。内容はChainerCVのSSD学習サンプルとだいたい同じです。
