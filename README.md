# Eureka Relaxation ホームページ

宮崎・橘通東の完全個室リラクゼーション「Eureka Relaxation」の1ページ公式サイト。
静的HTML1枚（`index.html`）だけで完結。ビルド不要。

## 公開URL（予定）
- https://eureka-salon.ynsysapp.com
- 予約アプリ（別）: https://eureka.ynsysapp.com

## 差し替え素材
- `images/access-1.jpg` `images/access-2.jpg` `images/access-3.jpg` … 道順の写真3枚
  （置くと道順セクションに自動表示。未設置ならプレースホルダ表示）
- コンセプトの `respire` 枠の写真（任意）

## リンク
- LINE友だち追加/予約: https://lin.ee/rqIuPEV
- Googleマップ: https://maps.app.goo.gl/8hctZVgHbTDUfBpM9

## デプロイ（Cloudflare Pages 推奨・独自ドメインはynsysapp.comがCloudflare管理のため自動連携）
### 方法A：フォルダを直接アップロード（GitHub不要・最速）
1. Cloudflare ダッシュボード → Workers & Pages → Create → Pages → 「Upload assets」
2. このフォルダ（index.html と images/）をアップロード → Deploy
3. 対象Pages → Custom domains → `eureka-salon.ynsysapp.com` を追加（DNSは自動設定）

### 方法B：GitHub連携（更新を自動反映したい場合）
1. このリポジトリをGitHubへ push（GitHub Desktop等）
2. Cloudflare Pages → Create → 「Connect to Git」→ 当リポジトリを選択（ビルド設定なし・出力ルート = /）
3. Custom domains → `eureka-salon.ynsysapp.com` を追加

更新時は index.html を編集して再アップロード（A）／push（B）。
