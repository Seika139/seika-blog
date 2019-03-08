# seika-blog
this blog is created as a study of DjangoGirls


---

#### 参考サイト

1. [仮想環境を使い分けることで`requirements.txt`に必要なライブラリだけを入れることができる。](https://qiita.com/mizoe@github/items/0f7898fe026fa4cefe9d)


  ```
  python -m venv heroku_env       # 仮想環境を作る(Python 3.3からの標準機能)
  source heroku_env/bin/activate  # 仮想環境をアクティベート
  pip install --upgrade pip       # pipアップグレード
  pip install django-toolbelt     # pipにDjangoインストール（他に必要なライブラリがあればそれも入れます）
  pip freeze > requirements.txt   # requirements.txtを再作成
  git add .
  git commit -m 'comment'
  git push heroku master          # デプロイ
  ```

2. [仮想環境の管理](https://qiita.com/fiftystorm36/items/b2fd47cf32c7694adc2e)

```
cd [project dir]
python3 -m venv [newenvname]      # 仮想環境を作る

source [newenvname]/bin/activate  # activate
deactivate                        # deactivate

pip install [package name]        # パッケージのインストール
pip freeze                        # 作成した環境にインストールされたパッケージの確認
```
