# k-space Mobile Simulator

スマートフォン対応のMRI k-space軌跡シミュレーターです。

## GitHub Pagesで公開する

1. GitHubで新しい **Public repository** を作成します。
2. このZIPを解凍し、ZIPの中身をすべてリポジトリ直下へアップロードします。
3. リポジトリの **Settings → Pages** を開きます。
4. **Build and deployment → Source** を **GitHub Actions** にします。
5. **Actions** タブで `Deploy static site to GitHub Pages` が完了するのを確認します。
6. **Settings → Pages** に表示されるURLをSafariで開きます。

公開URLは通常、次の形式です。

`https://GITHUBユーザー名.github.io/リポジトリ名/`

## iPhoneだけでアップロードする場合

SafariでGitHubを開き、リポジトリの **Add file → Upload files** を選択します。
ZIPそのものではなく、解凍後のファイルとフォルダをアップロードしてください。

最低限、次の構造を維持します。

```text
index.html
manifest.webmanifest
sw.js
.nojekyll
icons/
.github/
  workflows/
    pages.yml
```

## ホーム画面に追加

公開URLをSafariで開き、共有ボタンから **ホーム画面に追加** を選択します。

## 命令

- `MOVE kx ky`
- `READ kx ky samples`
- `BLIP dx dy`
- `WAIT n`
