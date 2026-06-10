# étoile（エトワール）公式サイト

東京都目黒区で活動する男女混合バレーボールチーム「étoile」の公式ホームページです。
HTML / CSS / JavaScript のみで構築された静的サイトで、GitHub Pages でそのまま公開できます。

## 構成

```
├── index.html      # トップページ（About / 入会案内 / 練習日程 / アクセス / Q&A）
├── terms.html      # サークル規約
├── css/style.css   # スタイルシート
├── js/main.js      # ナビゲーション・スクロールアニメーション
└── assets/
    └── mascot.png  # マスコット（ファビコン）
```

## GitHub Pages での公開手順

リポジトリ: https://github.com/Takumi1012/etoile_hp

1. リポジトリの **Settings → Pages** を開き、
   **Source: Deploy from a branch / Branch: main / フォルダ: (root)** を選択して保存
2. 数分後、`https://takumi1012.github.io/etoile_hp/` で公開されます

更新は `git push` するだけで数分後に自動反映されます。

独自ドメインを使う場合は Settings → Pages → Custom domain で設定できます。

## 写真の差し替え（推奨）

現在、About セクションの写真は Unsplash のフリー素材を使用しています。
チームの実際の写真に差し替えると、ぐっと魅力的になります。

| 場所 | 推奨サイズ | 差し替え方法 |
|---|---|---|
| Aboutセクション | 横1200px 程度（横長 4:3） | `assets/photo-about.jpg` を置き、`index.html` の `<img src="...">` を書き換え |
| ヒーロー背景（任意） | 横1920px 程度 | `css/style.css` の `.hero` の `background` に追加 |

おすすめの写真:
- 練習中のプレー写真（スパイク・レシーブの瞬間など動きのあるもの）
- 集合写真（イベントやÉtoile杯のもの）
- バーベキューなどイベントの楽しそうな雰囲気の写真

※ 人物が写っている写真を公開する場合は、メンバーの了承を得てください。

## 更新方法

- **練習日程**: Google カレンダー（既存の埋め込み）を更新すれば自動で反映されます
- **テキスト**: `index.html` / `terms.html` を直接編集してコミット & プッシュ
- **お問い合わせ**: 公式 LINE への導線に統一しています（静的サイトのためフォーム送信サーバーは不要）
