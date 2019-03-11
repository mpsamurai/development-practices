# Django Project

## settings.py のディレクトリ構造

settings.py のディレクトリ構造は下記のようにする。

```
sample_project
|- sample_project
  |- settings
    |- __init__.py
    |- base.py # 全環境共通
    |- develop.py # 開発環境共通
    |- staging.py # ステージング共通
    |- production.py # プロダクション共通
    |- local.py # ローカル環境独自
```

## Credentials

* クレデンシャルは、環境変数に保持して直接ソースコードには記載しない。
* 必要なクレデンシャルは、```settings```の中で```os.environ```などを用いて読み込む。
