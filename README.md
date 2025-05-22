# QianTa 電商管理系統

> 📖 [返回個人簡介](https://github.com/Qoo143/profile) | 🎯 轉職課程畢業作品

一個完整的全端電商管理系統，實現前後台分離架構，支援商品管理、購物車、訂單流程等核心電商功能。

## 🚀 專案連結

- **🌐 [前端專案](https://github.com/Qoo143/finall_front)** - Vue 3 + TypeScript
- **⚙️ [後端專案](https://github.com/Qoo143/finall_back)** - Express + MySQL

## 📋 解決的核心問題

### 電商系統完整功能
- **商品管理**：新增、編輯、刪除商品，支援圖片上傳與 3D 模型展示
- **購物車系統**：加入購物車、數量調整、即時計算總價
- **訂單流程**：下單、付款、訂單狀態管理
- **用戶管理**：會員註冊登入、訂單查詢

### 權限分離架構
- **一般用戶**：商品瀏覽、購物車、訂單管理
- **管理員**：後台商品管理、分類標籤管理、訂單處理
- **JWT 身份驗證**：確保 API 安全性

### 使用體驗優化
- **GSAP 滾動動畫**：主頁 ScrollTrigger 實現流暢視覺效果
- **響應式設計**：適配桌面與移動端
- **3D 商品展示**：Google Model Viewer 展示立體商品

## 🛠 技術架構

### 前端技術棧
```
Vue 3 (Composition API) + TypeScript
├── 狀態管理: Pinia
├── UI 框架: Element Plus
├── 路由管理: Vue Router
├── 動畫效果: GSAP + ScrollTrigger
├── 3D 展示: Google Model Viewer
└── HTTP 請求: Axios
```

### 後端技術棧
```
Express.js + MySQL
├── 身份驗證: JWT + bcryptjs
├── 檔案上傳: Multer
├── 資料驗證: Joi
├── API 設計: RESTful
└── 錯誤處理: 統一中間件
```

### 核心特色
- **3D 模型展示**：支援 GLB 格式商品模型
- **圖片處理**：多圖上傳、主圖設定、縮圖展示
- **狀態管理**：Pinia 實現購物車跨頁面狀態同步
- **動畫交互**：GSAP 實現首頁滾動視差效果

## 📊 API 設計概覽

### 商品管理 API
```
GET    /products          # 商品列表(支援篩選)
GET    /products/:id      # 商品詳情
POST   /products          # 新增商品
PUT    /products/:id      # 更新商品
DELETE /products/:id      # 刪除商品
```

### 購物車 API
```
GET    /api/cart          # 獲取購物車
POST   /api/cart/items    # 加入商品
PATCH  /api/cart/items/:id # 更新數量
DELETE /api/cart/items/:id # 移除商品
```

### 訂單管理 API
```
GET    /api/orders        # 訂單列表
POST   /api/orders        # 建立訂單
PATCH  /api/orders/:id/cancel # 取消訂單
```

### 用戶認證 API
```
POST   /api/register      # 用戶註冊
POST   /api/login         # 用戶登入
```

## 🎯 專案架構設計

### 前端模組化結構
```
src/
├── components/     # 可復用組件
├── views/         # 頁面組件
├── stores/        # Pinia 狀態管理
├── api/           # API 請求封裝
├── utils/         # 工具函數
└── types/         # TypeScript 型別定義
```

### 後端分層架構
```
├── router/                # 路由定義
├── router_controllers/    # 控制器邏輯
├── middleware/           # 中間件
├── db/                   # 資料庫連接
└── public/uploads/       # 檔案存儲
```

## 🚧 開發思路與挑戰

### 學習路徑
- **技術選擇**：研究各框架評論與發展趨勢，選擇 Vue 3 生態系
- **架構設計**：參考《Vue.js 設計與實現》等書籍，建立模組化架構
- **開發策略**：AI 輔助生成基礎代碼，再手動調整符合需求

### 技術難點解決
- **狀態同步**：Pinia 解決購物車跨頁面狀態管理
- **檔案上傳**：Multer 處理多圖片與 3D 模型上傳
- **權限控制**：JWT 中間件實現路由層級權限驗證
- **動畫性能**：GSAP 優化滾動動畫避免卡頓

### AI 輔助開發實踐
2個月完成全端專案的關鍵：**先求有，再求好**
- 透過 AI 快速生成 API 架構與基礎組件
- 手動優化業務邏輯與用戶體驗細節
- 重點放在功能完整性而非代碼完美度

## 📈 專案成果

- **開發週期**：2個月（學習4個月後）
- **代碼量**：前端約 15,000 行，後端約 8,000 行
- **功能完整度**：涵蓋電商核心流程
- **技術整合**：成功整合 10+ 技術棧

---

### 💡 開發心得

從零基礎到完成全端專案，最大的體悟是**時間管理**與**技術選擇**的重要性。通過 AI 輔助開發大幅提升效率，但更重要的是理解業務邏輯並做出正確的架構決策。這個專案讓我體驗到全端開發的挑戰與成就感。

> 📋 詳細說明請查看各專案儲存庫的 README 文件
