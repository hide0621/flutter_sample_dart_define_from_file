# flutter_sample_dart_define_from_file

このレポジトリは書籍「Flutter実践開発」第４章４節「dart-define-from-file 環境変数を扱う」の内容に基づくものです。

[Flutter実践開発 - iPhone／Android両対応アプリ開発のテクニック - ](https://gihyo.jp/book/2024/978-4-297-13993-3)

## コードと設定を分離するまでの手順

手順１：

  - 環境変数をJSON形式で記述する（詳しくはこのレポジトリの**プロジェクトルート**にある`define/env.json`を参照）

手順２：

  - 上記のファイルのパスを`Flutter`コマンドに渡すか、Android Studioで実行する際は「Runボタンの右側にある3点リーダー」→「Edit」→「Run/Debug Configrations」ウィンドウを開く

  - 「Additional run args」に「`--dart-define-from-file=`」に続いて上記のJSONファイルのパスを記述する

  - なお、**この設定はこのレポジトリ（プロジェクト）にのみ適用される**。別のプロジェクトやそれを動かすAndroid Studioには適用されない！

手順３：

  - `main`ファイルにある通り、環境変数をコードから参照するコードを書く

  - 詳しくは`main`ファイルのドキュメントコメントを参照

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
