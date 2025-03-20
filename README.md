# 2025_238571G_yabiku_review

# 研究題目：多角的な有用性評価に向けた商品タイプ別ラベル設計と不均衡データ改善に向けたデータ拡張手法の提案

## 実行環境

- Google colab
- pytorchなどのフレームワークバージョン情報は各ipynbファイル参照

## 手順
### 基礎実験
1. エクセルファイル上のデータセットの前処理：Colab_Notebooks内のLoad_〇〇.ipynbを実行する．reviewフォルダ内にcsvファイルが生成される．（生成済み）
2. 上記の作成されたデータセットを用いてファインチューニング： Learn_〇〇.ipynbを実行する．

### Focal loss
Learn_〇〇.ipynb冒頭のFocal lossをTureへ変更

### データ拡張
1. ChatGPT-API.ipynbにAPI keyを入力し，対象となるデータの拡張を行う．
2. Learn_〇〇.ipynb中の拡張数の見出し部分よりデータ拡張数の調整を行う．
3. 結果をplot.ipnbに入力し，実行する．

### Probing
1. Learn_single_label_review.ipynbを実行しシングルラベル分類モデルを前述のデータセットによるファインチューニングで構築．
2. 手順1で保存したモデルのパスをeval_single_label_model.ipynbに入力し，プロービングを行う．





