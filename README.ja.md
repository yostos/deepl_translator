# deepl_translator

`deepl_translator`は、DeepL API（無料版）を使用して英語と日本語のテキストを相互に翻訳するシンプルなコマンドラインツールです。このツールは、標準入力からテキストを受け取り、翻訳結果を標準出力に出力します。

## 特徴

- 英語から日本語、及び日本語から英語への翻訳サポート
- コマンドラインから簡単に使用可能
- `.env`ファイルを通じたAPIキーの簡単な設定

## 前提条件

- Python 3.x
- pip（Pythonのパッケージマネージャ）

## インストール

以下のコマンドを使用して、`deepl_translator`をインストールします：

bashCopy code

`pip install git+https://yourrepository.com/deepl_translator.git`

> 注: 上記のURLは、このパッケージをホストしているGitリポジトリのURLに置き換えてください。

## APIキーの設定

`deepl_translator`を使用する前に、DeepL APIの無料APIキーを取得し、`.env`ファイルに以下のように設定する必要があります：

1.  DeepL APIの無料アカウントをこちらから作成し、APIキーを取得してください。
2.  プロジェクトのルートディレクトリに`.env`ファイルを作成します。
3.  以下の内容を`.env`ファイルに追加し、`YOUR_API_KEY`をあなたのAPIキーに置き換えてください：

makefileCopy code

`DEEPL_API_KEY=YOUR_API_KEY`

## 使用方法

コマンドラインから`deepl_translator`を使用して、テキストファイルを翻訳します：

bashCopy code

`cat input.txt | deepl -t [target_language] > output.txt`

ここで、`[target_language]`は翻訳先の言語を指定します。オプションは以下の通りです：

- `j` または `japanese`：日本語に翻訳
- `e` または `english`：英語に翻訳

例えば、英語のテキストファイルを日本語に翻訳するには：

bashCopy code

`cat input.txt | deepl -t j > output.txt`

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。

## 貢献

貢献したい方は、プルリクエストを送るか、問題を報告してください。全ての貢献に感謝します！
