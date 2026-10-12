兵庫ベース運行情報チェッカー PWA v0.4.1 公開手順

【公開前に必ず確認】
・GitHub Pages（通常設定）はWeb上に公開されます。URLを知らなくても閲覧され得ます。
・このHTMLにはコース名（有吉・川上）、出発時刻、走行路線が含まれています。
・利用者ごとのアクセス制限はありません。親しい人限定で使わせたい場合は認証付き公開先が必要です。
・交通情報のリアルタイム自動取得・迂回路自動計算は未実装です。

【公開手順（GitHub Pages）】
1. GitHubにログイン https://github.com/
2. 右上の＋から New repository を選択。例: hyogo-truck-checker
3. 公開範囲 Public になることを承知のうえでリポジトリ作成（GitHub FreeのPagesを利用する場合）。
4. Add file → Upload files を選択。ZIPそのものではなく、展開後の index.html / sw.js / manifest.webmanifest / icon-192.png / icon-512.png / .nojekyll をルートにアップロード。
   ※.nojekyll は隠しファイルなので選択に出ない場合は省略可。READMEも任意。
5. Commit changes を押す。
6. Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root) → Save。
7. Pages欄に表示されたURLをAndroid Chromeで開く。
8. Chromeメニュー（︙）→「アプリをインストール」または「ホーム画面に追加」。

【注意】
・アプリの交通状況欄は自動的に最新データを取得していません。
・通信がなくても画面が起動する場合がありますが、公式リンクは通信が必要です。
・旧版を導入済みの場合、ブラウザのキャッシュに旧アイコンが残ることがあります。
・記録は利用者のブラウザに保存され、別端末とは同期されません。
