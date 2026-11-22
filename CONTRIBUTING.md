# Contributing

スキルの追加・変更は Pull Request (PR) で提案してください。

## 新しいスキルを追加する

1. `skills/<skill-name>/SKILL.md` を作成する
2. 補助資料は同じディレクトリの `references/` に置く
3. `SKILL.md` の front matter に `name` と `description` を記載する
4. ルート `README.md` の Skills 一覧を更新する
5. 個人情報・訪問履歴・位置情報・アカウント情報を含めない
6. 外部サービスの規約に反するスクレイピングやデータ再配布を前提にしない

## PR の流れ

- `feat/<skill-name>` または `update/<skill-name>` ブランチを作成
- スキル本体、参照資料、READMEを更新
- PRテンプレートに沿って、目的・変更点・検証方法・プライバシー確認を記載
- レビューと合意後にマージ

小さな修正でも、原則として main へ直接 push せず PR を利用してください。
