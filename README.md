# ゆらゆら シンボルアニメーション

参考デザインをもとに、2本の不完全な円形ライン、可変幅の半透明リボン、偏心・歪み、円周上を移動する太い部分を、ネイティブWebGLシェーダーで再現した静的ページです。

## 公開ページ

https://mizukioyama.github.io/test-animation/

## 構成

- `index.html`：GitHub Pagesの入口。GPUで描画するWebGL実装
- `yurayura_symbol_animated.html`：アニメーション本体の保存版（入口と同一実装）
- `yurayura_symbol_preview.html`：初期デザインの静的プレビュー
- `yurayura_symbol_live_preview.html`：入口へ移動する互換ページ

外部API・ビルドツール・有料サービス・外部CDNは使用していません。WebGL非対応環境ではCanvas 2Dへフォールバックし、`prefers-reduced-motion` が有効な環境でも低速で再生します。`main`への反映後、GitHub Pagesの公開内容へ自動反映されます。
