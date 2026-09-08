Bar BlueTemple PRO v11 FIXED

今回の原因
v9/v10の script.js に余分な「});」が1か所あり、
JavaScript全体が構文エラーになっていたため、
YES/NOを含むボタン処理が全部停止していました。

修正
- script.js の構文エラーを修正
- Node.jsで構文チェック済み
- YESボタン動作を確認するコード構造を維持
- NOボタンの逃走処理を維持
- CSS/JSは ?v=11 でキャッシュ更新
- answer.htmlの直接表示はindexへ戻す
- YES経由のみ使い捨てトークンを発行
- SafariのBFCache復元時もindexへ戻す

GitHub PagesにはZIPの中身をすべて上書きしてください。
