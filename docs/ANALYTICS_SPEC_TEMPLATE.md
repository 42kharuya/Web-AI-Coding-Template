# Analytics Spec Template（イベント/プロパティ/KPI）

このテンプレは「最小の計測」を先に決めて、実装と運用を楽にするためのものです。

## 1) 北極星指標（North Star）

- 指標名:
- 定義（1文）:
- なぜこれか:

## 2) KPI（最初の2週間）

- アクティベーション率: activation users / signup users
- 継続率（例）: D7 active / D0 cohort
- 課金率（課金するなら）:

## 3) イベント一覧（最低限）

| event_name | いつ発火         | 目的     | 必須プロパティ        | 任意プロパティ |
| ---------- | ---------------- | -------- | --------------------- | -------------- |
| signup     | 登録完了時       | 獲得計測 | user_id, method       | referrer       |
| activation | 初回成功体験完了 | 価値検証 | user_id, step         | time_to_value  |
| purchase   | 購入/申込完了    | 収益計測 | user_id, plan, amount | coupon         |

### 命名ルール

- 小文字 + snake_case
- 意味が被るイベントを増やさない（迷ったら統合）

## 4) プライバシー/取り扱い注意

- 収集しない情報（PII/機微情報）:
- 保存期間:
- 同意（必要なら）:
