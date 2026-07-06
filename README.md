# 高橋 航 — Portfolio

建設コンサルタントの実務者でありAIツールの作り手、高橋航のポートフォリオサイト。
ビルド不要の単一HTML。`index.html` をブラウザで開くだけで動作します。

**Live:** _(Vercel URL をここに記載)_

## 構成

| セクション | 内容 |
|---|---|
| Hero | Spline製インタラクティブ3Dロボット + スポットライト |
| About | プロフィール |
| Works | 制作した業務AIツール |
| Approach | つくり方の3原則 |
| Contact | 連絡先 |

## 技術

- 単一 HTML + インライン CSS/JS(フレームワーク・ビルド不要)
- 3D: [Spline](https://spline.design/) の `spline-viewer` Web Component(CDN読み込み)
- 3Dシーンは `robot.splinecode` として**自己ホスト**(外部URL依存なし)
- フォント: Inter / Noto Sans JP / JetBrains Mono(Google Fonts)

## ローカル確認

```bash
python -m http.server 4173
# → http://localhost:4173
```

## ライセンス / クレジット

- **サイトのコード**(HTML/CSS/JS): 高橋航
- **Spline ラッパーの発想元**: [interactive-ui](https://github.com/coding-dada/interactive-ui)(MIT License）を参考にした独自実装
- **3Dロボットシーン** (`robot.splinecode`): Spline のデモ/コミュニティ素材。個人ポートフォリオでの埋め込み用途として利用。素材の再配布・再販は行っていません。完全に権利フリーな素材へ差し替える場合は [Spline Community の CC0 ロボット](https://community.spline.design/tag/robot) から入手可能です。
- **`spline-viewer` ランタイム**: © Spline（CDN経由で読み込み）
