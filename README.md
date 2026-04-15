# DefenseWatch Japan 🛡

防衛・軍事・安全保障ニュースを日本語でお届けするブログ。

**公開URL:** https://dai35room.github.io/defense-watch-japan/

---

## 初回セットアップ

### 1. Python パッケージのインストール
```bash
pip3 install feedparser requests
```

### 2. GitHubリポジトリを作成してpush
```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
git remote add origin https://github.com/dai35room/defense-watch-japan.git
git push -u origin main
```

### 3. GitHub Pages を有効化
GitHubリポジトリ → Settings → Pages →
**Source: GitHub Actions** を選択して Save

---

## 日常の使い方

### ① 新着ニュースを自動取得（下書き生成）
```bash
python3 auto_draft.py
```
→ `drafts/` に下書きHTMLが自動生成される

接続テスト：
```bash
python3 auto_draft.py --test
```

### ② $��書きを確認・編集
`drafts/` フォルダ内の `.html` ファイルをブラヰザで開いて確認。