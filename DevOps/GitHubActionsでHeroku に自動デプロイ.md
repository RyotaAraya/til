# 背景
実務でサブのCI/CDを改善したいと考えている。サブは昔作られたものでほぼノーメンテで稼働している。リリースログの集計時にメインとサブが分かれていると面倒なのとアカウント管理も煩雑になるため統一したい。
最終的にはメインとサブを同じフローにしたいと考えている。(GitHub→GitHubActions→Heroku)
ひとまずサブをGitHub→GitHubActions→Herokuに移行するため。実験したい。

メイン：GitHub→Travis→Heroku
サブ：Bitbucket→Jenkins→Heroku

# 目的
GitHub→GitHubActions→Herokuの自動デプロイを試す


# やったこと
- Hrokuの自動自動デプロイをデタッチする(既存 GitHub→Heroku)
- リポジトリにymlファイルを作成(API_KEYやAPP名などをsecretsに記載)
- commit

https://github.com/RyotaAraya/ts-nextbook-json


# おわりに
複雑な設定なしで簡単に動作を確認できた。GitHubからActionsのログを確認できるのも統一性があって便利。

# 参考
https://zenn.dev/shin_shin_01/articles/53009a81728e21
