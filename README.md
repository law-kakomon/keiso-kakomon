# 刑事訴訟法過去問帳

ロースクール既修者入試（刑事訴訟法）の過去問を、**刑訴の単元ごとに**引ける学習帳。

**https://law-kakomon.github.io/keiso-kakomon/**

- **単元から引く** — 捜査／公訴／公判／証拠／裁判・上訴
- **条文から引く** — 検索欄に `220` と入れると、220条が論じられている回が並ぶ
- **論点・判例で探す** — 「違法収集証拠」「最決昭和51年3月16日」などで検索
- **問題と解説をその場で読む** — 同志社・立命館は PDF をページ内に表示。慶應・中央はサーバー側の設定で埋め込めないため新しいタブで開く
- **解いた回に印をつける** — チェックはこの端末のブラウザにだけ残る

収録は京大・同志社・立命館・慶應・中央の5校、計 62 回（2005〜2027年度）。
立命館は2018・2019年度だけ「訴訟法オプション試験」として刑訴を出題していた（6回）。
関学は既修者入試で刑事訴訟法を課していないため、収録対象外。

**PDF は各大学の公式ページをそのまま開きます**（このリポジトリに複製は置いていません）。

## 使い方

上の URL をブラウザで開くだけ。スマホでは「ホーム画面に追加」するとアプリのように使える。

手元で動かすとき:

```bash
open 開く.command
```

## 更新

```bash
python3 tools/fetch_sources.py   # 各大学のページを見て新年度を拾う
python3 tools/digest.py <id>     # 新しい回の条文・判例・論点を取り出す
# → 出力を見て tools/classify.py に単元を書く
python3 tools/build_data.py      # data/kakomon.json と index.html への埋め込みを作り直す
```

## 姉妹サイト

科目の入口は **https://law-kakomon.github.io/** 。

- [民法過去問帳](https://law-kakomon.github.io/minpo-kakomon/)
- [民事訴訟法過去問帳](https://law-kakomon.github.io/minso-kakomon/)
- [会社法過去問帳](https://law-kakomon.github.io/kaisha-kakomon/)
- [憲法過去問帳](https://law-kakomon.github.io/kenpo-kakomon/)
- [行政法過去問帳](https://law-kakomon.github.io/gyosei-kakomon/)
- [刑法過去問帳](https://law-kakomon.github.io/keiho-kakomon/)
