# SUBWORTH — Legal / Support

iOS アプリ「SUBWORTH」（リポジトリ名は `subcut-app`）の、プライバシーポリシーと
サポートページ。GitHub Pages で公開し、App Store Connect に URL を登録する。

ASC の主言語は **English (U.S.)** なので、**ルートを英語**、`ja/` を日本語にしてある。
ASC の URL 欄はローカライズごとに設定できるので、言語別に出し分ける。

| ローカライズ | サポート URL | プライバシーポリシー URL |
|---|---|---|
| English (U.S.) | `.../support.html` | `.../privacy-policy.html` |
| 日本語 | `.../ja/support.html` | `.../ja/privacy-policy.html` |

```
index.html              言語のハブ
privacy-policy.html     English
support.html            English
ja/privacy-policy.html  日本語
ja/support.html         日本語
```

## 直すとき

**日英を対で直す。**片方だけ更新すると、言語で書いてあることが食い違う。
最終更新日も両方書き換える。

無料枠・通知のタイミング・Pro の内容は本体リポジトリの実装が正。
`lib/domain/pro/pro_policy.dart` と `lib/domain/notifications/reminder_plan.dart` を
変えたら、このページの記述も合わせる。

## 公開

GitHub の Settings → Pages で `main` ブランチのルートを公開する。
