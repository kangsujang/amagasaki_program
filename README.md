# 授業リンク集

中学生向けの授業で使うリンク集です。`index.html` 1ファイルだけで動きます（外部ライブラリ・広告・アクセス解析なし）。

## リンクの編集

`index.html` をテキストエディタで開き、各教科の `<ul class="links">` の中に次の1行を追加します。

```html
<li><a href="https://example.com" target="_blank" rel="noopener">サイト名<span>説明文</span></a></li>
```

教科を増やすときは `<section>` をまるごとコピーし、`id` と見出しを変え、上部の `<nav>` にもリンクを追加してください。
編集後は、ファイルをブラウザで開けば表示を確認できます。

## 無料で公開する（GitHub Pages）

1. GitHub アカウントを作成（無料）
2. 新しいリポジトリを **Public** で作成（例: `amagasaki_program`）
3. このフォルダで次を実行

   ```bash
   git init -b main
   git add index.html README.md
   git commit -m "授業リンク集を作成"
   git remote add origin https://github.com/<ユーザー名>/amagasaki_program.git
   git push -u origin main
   ```

   コマンドを使わない場合は、GitHub の画面で「Add file → Upload files」から `index.html` をアップロードしても構いません。
4. リポジトリの **Settings → Pages** で、Source を「Deploy from a branch」、Branch を `main` / `/(root)` にして Save
5. 1〜2分後、`https://<ユーザー名>.github.io/amagasaki_program/` で公開されます

以後は `index.html` を更新して push（またはアップロード）するだけで、サイトに反映されます。

## 注意

- 検索エンジンに載らないよう `noindex` を設定しています。URLを知っている人は誰でも見られるので、個人情報や校内限定の情報は載せないでください。
- 学校のネットワークでフィルタリングされるサイトもあるため、授業前に生徒用端末で開けるか確認してください。
