# 提案審查分析系統

上傳徵求資料 + 廠商提案，AI 自動產出結構化審查意見。

## 部署步驟（Vercel）

### 1. 上傳到 GitHub
1. 到 https://github.com → New repository → 命名 `proposal-reviewer` → Create
2. 上傳此資料夾所有檔案（直接拖曳到 GitHub 網頁）

### 2. 部署到 Vercel
1. 到 https://vercel.com → 用 GitHub 登入
2. Add New Project → 選 `proposal-reviewer`
3. 直接按 **Deploy**（不需要改任何設定）

### 3. 設定 API Key（重要）
部署完成後：
1. 進入 Vercel 專案 → **Settings** → **Environment Variables**
2. 新增一筆：
   - Name：`ANTHROPIC_API_KEY`
   - Value：你的 `sk-ant-api03-...` 金鑰
3. 按 **Save** → 回到 **Deployments** → **Redeploy**

完成！你的網址會是 `https://proposal-reviewer-xxx.vercel.app`
