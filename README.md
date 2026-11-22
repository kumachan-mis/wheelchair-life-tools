# wheelchair-life-tools

車いす利用者が外出先を自分の条件で判断するための、再利用可能な支援スキル集。

## Skills

### `restaurant-entry-research`

飲食店の入店可否を、一般的な「車いす可」表示だけに頼らず、道路から着席場所までの経路・段差・入口幅・エレベーター・介助条件に分けて調査するスキル。

- [スキル本体](skills/restaurant-entry-research/SKILL.md)
- [入店レベル基準](skills/restaurant-entry-research/references/entry-level.md)
- [既知施設データのローカルテンプレート](skills/restaurant-entry-research/references/known-places.md)

## 使い方

対応するエージェント／スキルランタイムに `skills/restaurant-entry-research/` を登録してください。
最初に `references/entry-level.md` を利用者本人の車いす・介助条件に合わせて確認・調整してください。

`references/known-places.md` は利用者ごとのローカルデータです。訪問履歴や個別判定を公開リポジトリへ追加せず、ローカルコピーで管理してください。

## 設計原則

- 利用者本人の実地判断をAIの推定や一般的なアクセシビリティ表示より優先する
- 物理的な入店難易度と、今回の同行者・介助条件での可否を分ける
- 道路から着席場所までを区間ごとに評価する
- 写真で確認できた事実、推定、未確認事項を明確に分ける
- 写真や外部サイトの規約を尊重し、無断スクレイピング・再配布をしない
- 不明な点を断定せず、結論を左右する未確認事項を具体的に示す

## Contributing

新しいスキルの追加・既存スキルの変更は、原則としてブランチを作成し Pull Request で提案してください。
詳細は [CONTRIBUTING.md](CONTRIBUTING.md) を参照してください。
