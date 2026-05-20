# Gitミニガイド

## 基本の流れ

```bash
# 1. ブランチを作成して移動
git checkout -b members/taro

# 2. ファイルを編集後、ステージング
git add members/taro.md

# 3. コミット
git commit -m "Add taro's profile"

# 4. プッシュ（初回）
git push origin members/taro
```

その後 GitHub で Pull Request を作成する。

## よく使うコマンド

| コマンド | 説明 |
|---|---|
| `git clone <URL>` | リポジトリをローカルにコピーする |
| `git checkout -b <ブランチ名>` | 新しいブランチを作成して移動する |
| `git status` | 現在の状態を確認する |
| `git add <ファイル>` | 変更をステージングする |
| `git commit -m "メッセージ"` | コミットする |
| `git push origin <ブランチ名>` | リモートにプッシュする |
| `git pull` | リモートの変更を取り込む |

## コンフリクトが起きたら

同じファイルを複数人が編集すると、マージ時にコンフリクトが発生します。

```bash
# 1. main の最新を取り込む
git pull origin main

# 2. コンフリクトしているファイルを開いて編集する
#    <<<<<<< HEAD  ← 自分の変更
#    =======
#    >>>>>>> main  ← 相手の変更
#    この部分を手動で整理して保存する

# 3. 解決後にコミット
git add <ファイル>
git commit -m "Resolve conflict"
```

## 困ったら

- エラー文を読む
- チームメンバーに相談する
