# Start Here（初学者向け：2〜4週間でMVPを出す一本道）

このテンプレは「迷いを減らして最短で検証する」ための型です。
まずは **コア体験を1つ**に絞って、2〜4週間で出すことを優先します。

## 0) 今日やること（60〜120分）

1. [docs/PRD_TEMPLATE.md](PRD_TEMPLATE.md) を埋める（MVP / Won’t / KPI / Kill criteria まで）
2. [docs/architecture.md](architecture.md) に「最小設計」を1つだけ残す（ADR 0001）
3. [docs/MVP_BACKLOG_TEMPLATE.md](MVP_BACKLOG_TEMPLATE.md) を見ながら Issue を10〜20個に切る

> 迷ったら「やらないこと（Won’t）」を増やしてください。

---

## 1) 企画（Day 1）

編集: [docs/PRD_TEMPLATE.md](PRD_TEMPLATE.md)

完了条件（AC）

- [ ] コア体験が1文で言える
- [ ] MVP機能（Must）が3〜7個に収まっている
- [ ] Kill criteria（失敗判定）が明文化されている
- [ ] KPIが2週間で測れる形になっている

---

## 2) 設計（Day 1〜2）

編集: [docs/architecture.md](architecture.md)

完了条件（AC）

- [ ] 画面（ページ）一覧がある
- [ ] データ（テーブル/ドキュメント）の最小モデルがある
- [ ] リスク（規約/個人情報/支払い/依存）と回避策が1行ずつある

---

## 3) 計測設計（Day 2）

編集: [docs/ANALYTICS_SPEC_TEMPLATE.md](ANALYTICS_SPEC_TEMPLATE.md)

最低限、次だけ定義してください。

- signup（登録）
- activation（初回成功体験）
- purchase（課金するなら）

KPI例:

- アクティベーション率 = activation / signup

---

## 4) 実装（Week 1〜2）

運用: GitHub Issues + PR（[.github/pull_request_template.md](../.github/pull_request_template.md)）

ルール

- 1 Issue = 1 PR
- PRは「半日以内に終わる粒度」に切る
- 重要導線（登録→初回成功体験→課金）以外は後回し

---

## 5) ローンチ準備（Week 2〜3）

編集: [docs/LAUNCH_CHECKLIST.md](LAUNCH_CHECKLIST.md) / [docs/RUNBOOK_TEMPLATE.md](RUNBOOK_TEMPLATE.md)

完了条件（AC）

- [ ] 問い合わせ導線がある（[SUPPORT.md](../SUPPORT.md)）
- [ ] 規約・プライバシー方針が用意できる（文面は別途）
- [ ] ロールバック手順が箇条書きである

---

## 6) マーケ/改善（Week 3〜4）

編集: [docs/GROWTH_PLAYBOOK.md](GROWTH_PLAYBOOK.md)

完了条件（AC）

- [ ] 7日分の投稿計画がある
- [ ] 改善実験が週3本のペースで回せる（仮説→実施→計測→学び）
