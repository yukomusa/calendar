# vscode-devcontainer-python-base

vscode で dev container を使って python の開発をするためのテンプレート

### 事前準備

- vscode に拡張 "Remote Development" をインストールしておく
- Docker Desktop をインストールして起動しておく

### 使い方

1. プロジェクト始める（プログラムを書き始める）時、このレポジトリテンプレートからプロジェクト名のレポジトリを作成する。
1. 作成したレポジトリをローカル環境（PC）上に clone する。
1. ローカルのレポジトリで vscode を開く

```
code ディレクトリ
```

4. vscode 左下の `><` こんなアイコンをクリックして `Reopen in container` を選択すると、python が実行可能なコンテナ内で vscode が開かれる
5. コンテナ内でプロジェクトが開かれているときは 左下の領域は `>< Dev Container: プロジェクト名` のようになっているので、時々確認すること。
6. プログラムを書く
7. 書いたプログラムを確認してもらうときは、そのレポジトリ/ブランチを push するなり、PR をだすと、確認者はそのレポジトリ/ブランチを使ってすぐに動作確認ができる。
8. コンテナ内での作業を終えるときは `><` から `Reopne folder localy` を選択する。作業してないときは Docker Desktop は終了しておく（無駄に PC 上の領域を専有するため）。

### その他

#### ライブラリを追加する時

- requirements.txt を編集して（追加するライブラリ名、バージョンを書く。例えば ↓）

```
geojson==3.0.1
```

- `><` アイコンをクリックして、`Rebuild Container` を選択する。vscode が再度開かれると、ライブラリが利用可能になっている。
## Demoの動かし方
このDemoはStreamlitが入っていることを前提に進みます

1. token.jsonとcredentials.jsonをワーキングディレクトリに保存する
2. 上の説明を読んでContainer内でこのプロジェクトを開く
3. ターミナルに以下のコマンドを打つ
```
streamlit run main.py
```
4. ブラウザ上でアプリが実行される  

### 空き時間を抽出する
1. 誰と誰のマッチングを行うか選択する  
今回は2人しかいません
2. 必要項目を選択し、空き時間を抽出のボタンをクリック

### 予定を作成する
1. 必要項目を入力する(このとき必ず説明をよく読んでください)
2. 予定を作成するボタンをクリック
3. Aivalix.calendar.app.demo@gmail.comのカレンダーが更新されます