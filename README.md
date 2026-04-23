# Autonomous Driving Decision Simulator

確率的意思決定に基づいて、前方車両との距離・車線状況・速度差を考慮しながら自車の行動を選択する、ブラウザベースの自動運転シミュレーターです。

## Overview

このプロジェクトは、HTML5 Canvas と JavaScript を用いて実装した自動運転意思決定シミュレーターです。
自車は周囲の状況を評価し、**直進・減速・停止・左車線変更・右車線変更**の中から確率的に行動を選択します。

## Features

- 確率分布に基づく行動選択
- 車線ごとの前方距離評価
- 衝突防止のための安全距離制御
- 車線変更時の安全性チェック
- Canvas ベースのリアルタイム可視化
- 現在速度、行動確率、EV、累積統計の表示

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- HTML5 Canvas

## How to Run

1. このリポジトリを clone または download します。
2. `autonomous-driving-simulator.html` をブラウザで開きます。
3. `▶ 시작` ボタンを押すとシミュレーションが始まります。

## Project Purpose

このプロジェクトは、確率的意思決定、簡易交通物理、リアルタイム可視化を組み合わせたフロントエンドシミュレーションの実装例として制作しました。
日本就職向けポートフォリオとして、JavaScript による状態管理・ロジック設計・デバッグ改善の流れが分かるように構成しています。

## Notes

- 単一 HTML ファイルで動作するため、セットアップなしで実行できます。
- 外部ビルドツールやフレームワークは使用していません。
- シミュレーションロジックは学習・ポートフォリオ目的で実装しています。

## Author

Ajou University Software Student / Portfolio Project
