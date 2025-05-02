# Contributing

このリポジトリでは次のブランチ運用モデルを採用しています：

- **main**: 本番デプロイ済みの安定版
- **develop**: 次期リリース候補を統合
- **feature/**: 個別機能・修正ごとに作成
  - `git checkout -b feature/xxx develop`
  - 開発 → コミット → `git push -u origin feature/xxx`
  - GitHub 上で Pull Request → develop にマージ
- **release/** (任意): リリース前の最終調整用
- **hotfix/** (任意): 本番緊急修正用

## ワークフロー例

1. `develop` を最新化  
2. `feature/xxx` ブランチを作成  
3. 開発・コミット・プッシュ  
4. Pull Request → `develop` へマージ  
5. QA・テスト  
6. `develop` → `main` にマージ → デプロイ
