# Git/GitHubチュートリアル用

このリポジトリは、Git / GitHub を使ったチーム開発の練習用です。

チュートリアルの詳細は、システム創成プロジェクトNotion内の情報を参照してください。

## 目的

- ブランチと Pull Request を使った開発フローを体験する
- チームで変更を管理する

## 最初にやること

### チーム代表者

1. 画面右上の **Use this template** > **Create a new repository** から新規リポジトリを作成
2. 作成したリポジトリで、チームメンバを collaborator として追加する
   - リポジトリの Settings > Collaborators > Add people

### 全員（上記リポジトリに参加後）

1. リポジトリを clone する
2. 作業用ブランチを作成する（例：`git checkout -b members/taro`）
3. 自分の自己紹介ページを作る
4. 変更を add → commit → push する
5. Pull Request を出す

## ルール

- main ブランチに直接 push しない
- 必ず Pull Request (PR) を使う
- PR には説明を書く
- PR は他のメンバー 1 名以上が確認してからマージする

## ミッション

- [members/README.md](members/README.md) に従って自己紹介ページを追加する
- `index.html` にリンクを追加する（※コンフリクトが起きたら [git-guide.md](docs/git-guide.md) を参考に解決してみよう）
- 他人のページを改善する（誤字修正・情報追加など）
