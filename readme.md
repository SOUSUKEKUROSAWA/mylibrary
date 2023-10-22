# わたしの図書館
## 概要
## 開発

python仮想環境の起動
```bash
Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope Process
```
```bash
. venv/Scripts/activate
```

ローカルで動作確認
```bash
python manage.py runserver
```

ディレクトリ構造
```
mylibrary/
├── manage.py
├── project/
└── book_log/
```
- manage.py
  - Djangoプロジェクトとそのコンポーネントを管理するためのコマンドラインユーティリティ
- project/
  - プロジェクトレベルの設定
- book_log/
  - 自分が読んだ本の感想などをログとして保存する機能

パッケージの更新
```bash
pip install <package name>
```
```bash
pip freeze > requirements.txt
```

Python Anywhereへのデプロイ

1. **Python Anywhereにサインアップし、新しいウェブアプリケーションを作成**

2. **コードをアップロード**
    - GitHubなどを使用してコードをアップロードします。

3. **WSGIファイルの設定**
    - Python Anywhereの管理画面でWSGIファイルを設定します。

4. **静的ファイルの設定**
    - `settings.py`で`STATIC_URL`と`STATIC_ROOT`を設定し、`collectstatic`を実行します。

5. **Webアプリケーションのリロード**
    - Python Anywhereの管理画面でリロードをクリックします。

以上の手順は一例です。特定の要件や課題に応じて適宜カスタマイズしてください。