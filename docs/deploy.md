# GitHub Pages でのデプロイ方法

あなたのリポジトリ `https://github.com/atman-33/react-tailwind-ts-starter` を **GitHub Pages で公開**するには、以下のステップを順番に実行すればOKです。

---

## ✅ 1. `vite.config.ts` に base パスを設定

リポジトリ名が `react-tailwind-ts-starter` のため、**`vite.config.ts` に base を明示的に指定**します：

```ts
// vite.config.ts
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

// ✅ GitHub Pages用にbaseを指定
export default defineConfig({
  base: '/react-tailwind-ts-starter/',  // これを追加！
  plugins: [react()],
})
```

---

## ✅ 2. `gh-pages` パッケージをインストール

```bash
npm install --save-dev gh-pages
```

---

## ✅ 3. `package.json` にデプロイスクリプトを追加

```jsonc
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview",
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
  }
}
```

---

## ✅ 4. デプロイ実行

```bash
npm run deploy
```

これで、ビルドされた静的ファイル（`dist/` フォルダ）が `gh-pages` ブランチに push されます。

---

## ✅ 5. GitHub Pages の設定

GitHubのリポジトリに戻って：

1. `Settings > Pages` に移動
2. **Source** を `gh-pages` ブランチに変更
3. Folder は `/ (root)` を選択
4. 数十秒後に以下URLでアクセス可能になります：

👉 `https://atman-33.github.io/react-tailwind-ts-starter/`

---

## ✅ 6. Teams manifest.json に記載するURL例

```json
{
  "contentUrl": "https://atman-33.github.io/react-tailwind-ts-starter/",
  "websiteUrl": "https://atman-33.github.io/react-tailwind-ts-starter/"
}
```
