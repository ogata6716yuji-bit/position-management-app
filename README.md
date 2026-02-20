# Position Manager - PWA

ポジション管理システム（完全版）

## 📱 機能

- 18人のメンバー管理（A～R）
- 1～20のポジション管理
- タイマー機能（10～60分）
- リアルタイム日付・時刻表示
- アラート通知（音声・点滅・ブラウザ通知）
- 確認ダイアログ（移動・取消時）
- 一括リセット機能
- 日本語⇔英語切り替え
- 完全オフライン対応
- PWA対応（ホーム画面に追加可能）

## 📦 ファイル構成

```
position-manager-final/
├── index.html           # メインアプリ（確認ダイアログ付き）
├── manifest.json        # PWA設定
├── service-worker.js    # オフライン機能
├── icon-512.png         # アプリアイコン（赤い丸に3人と時計）
└── README.md           # このファイル
```

## 🚀 GitHub Pagesへのデプロイ

### 1. GitHubリポジトリ作成

1. https://github.com にログイン
2. 右上の「+」→「New repository」
3. Repository name: `position-manager` (任意)
4. **Public** を選択
5. 「Create repository」をクリック

### 2. ファイルアップロード

**重要：古いファイルがある場合は全て削除してから！**

1. 「Add file」→「Upload files」
2. 以下の4つのファイルを全てドラッグ&ドロップ：
   - index.html
   - manifest.json
   - service-worker.js
   - icon-512.png
3. 「Commit changes」をクリック

### 3. GitHub Pages設定

1. 「Settings」タブをクリック
2. 左メニューから「Pages」をクリック
3. Source設定：
   - Branch: **main**
   - Folder: **/ (root)**
4. 「Save」をクリック
5. 数分待つと、URLが表示されます：
   ```
   https://ユーザー名.github.io/position-manager/
   ```

## 📱 スマホでインストール

### iPhone (Safari)
1. 上記URLをSafariで開く
2. 画面下部の「共有」ボタン（□↑）をタップ
3. 「ホーム画面に追加」をタップ
4. 「追加」をタップ
5. ✅ ホーム画面にアイコンが表示されます！

### Android (Chrome)
1. 上記URLをChromeで開く
2. 画面下部に「ホーム画面に追加」または「インストール」が表示される
3. タップしてインストール
4. ✅ ホーム画面にアイコンが表示されます！

## 🔄 アプリの更新方法

### ファイルを更新する場合

1. GitHubのリポジトリで更新したいファイルをクリック
2. 鉛筆アイコン（Edit）をクリック
3. 内容を編集
4. 「Commit changes」をクリック
5. 数分で更新が反映されます

### スマホで更新を反映

1. アプリを一度削除
2. ブラウザのキャッシュをクリア
3. URLに再度アクセス
4. 再インストール

## 💡 トラブルシューティング

### アイコンが表示されない
- 全てのファイルが同じフォルダにあるか確認
- ファイル名が正確か確認（大文字小文字も一致）
- ブラウザのキャッシュをクリア

### インストールできない
- HTTPSでアクセスしているか確認（GitHub Pagesは自動的にHTTPS）
- manifest.jsonが正しくアップロードされているか確認
- Service Workerが登録されているか確認（ブラウザのデベロッパーツールで確認）

### 横向きにならない
- manifest.jsonのorientationが"any"または未設定になっているか確認

## ✅ 完成

ホーム画面から一発起動できる、完全なPWAアプリの完成です！

---

**開発:** Claude & User  
**バージョン:** 1.0  
**更新日:** 2026年2月
