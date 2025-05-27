<div align="center">
  
# 🚗 QianTa 汽車商城全端專案

![Vue.js](https://img.shields.io/badge/Vue.js-3.5-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white) ![Express](https://img.shields.io/badge/Express-4.21-000000?style=for-the-badge&logo=express&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

*完整的電商管理系統 | 前後台分離架構 | 轉職學習成果*

</div>

---

## 🎬 專案演示影片 (連結到外部)

<div align="center" width="600px">

[![QianTa 電商系統完整演示](docs/screenshots/frontend/home_index.png)]([https://www.youtube.com/watch?v=esLdX9oOl5s&list=RDesLdX9oOl5s&start_radio=1&ab_channel=HuaChenyu](https://www.youtube.com/watch?v=psT2QZBZMmo&ab_channel=ooQ)

*點擊上方圖片觀看完整功能演示*

</div>

---

## 🎯 專案快速簡介

QianTa 是一個功能完整的汽車電商系統，提供前台購物體驗和後台管理功能。

用戶 : 可以瀏覽汽車商品、3D預覽、加入購物車、完成模擬結帳；

管理員 : 可以進行商品一系列管理操作。

### 核心特色
- 🛒 **完整購物流程** - 商品瀏覽 → 購物車 → 結帳 → 訂單管理
- 🎭 **3D商品展示** - model-viewer 實現立體商品預覽
- 🔄 **商品管理** - 後台可讓管理員對產品相關資料做編輯  
- 🎨 **動畫效果** - GSAP ScrollTrigger 打造流暢滾動體驗
- 🔐 **權限控制** - JWT 身份驗證，前後台角色區分

---

## 📊 專案數據

- **開發週期**：2個月AI輔助開發
- **學習時程**：4個月從零基礎開始自學
- **總共時程**：共計6個月完成學習與開發
- **API接口**：20+ 個 RESTful 接口
- **數據表**：12 個核心業務表

---

## 🔗 專案連結 (查看前端與後端原碼)

- **🌐 [前端專案](https://github.com/Qoo143/finall_front)** - Vue 3 + TypeScript
- **⚙️ [後端專案](https://github.com/Qoo143/finall_back)** - Express + MySQL

---

## 🛠 技術架構

### 前端技術棧
```
Vue 3 + TypeScript + Pinia
├── UI框架: Element Plus
├── 動畫: GSAP + ScrollTrigger + VueTransition
├── 3D展示: Google Model Viewer
├── 狀態管理: Pinia Store
├── 路由管理: Vue Router
└── 樣式處理: SCSS
```

### 後端技術棧
```
Express.js + MySQL
├── 身份驗證: JWT + bcryptjs
├── 檔案上傳: Multer
├── 資料驗證: Joi
├── 資料庫: MySQL
├── API設計: RESTful
└── 錯誤處理: 統一中間件
```

### 架構設計理念
- **前後端分離**：Vue SPA + Express API Server，職責清晰分離
- **數據庫設計**：關聯式設計，支援商品、用戶、訂單完整關聯
- **身份驗證**：JWT Token 機制，支援前後台權限控制
- **檔案管理**：支援商品圖片、3D模型檔案上傳存儲

---

## 🔧 網頁建置挑戰

### 購物車狀態
**挑戰**：用戶在不同頁面間購物車數據需保持一致  
**解決**：Pinia Store + localStorage 持久化存儲

### 多類型檔案與編輯一次處理  
**挑戰**：商品需同時上傳多張圖片和3D模型檔案  
**解決**：Multer中間件 + 事務處理確保數據完整性

### 權限控制
**挑戰**：前台用戶與後台管理員權限區分  
**解決**：JWT Token攜帶角色信息 + 路由中間件驗證

### 3D模型展示
**挑戰**：商品3D模型在瀏覽器中展示  
**解決**：Google Model Viewer + GLB格式支援

---

## 📋 功能清單

### 前台功能
- ✅ 用戶註冊登入
- ✅ 商品瀏覽搜索  
- ✅ 3D商品預覽
- ✅ 購物車管理
- ✅ 結帳流程
- ✅ 訂單查詢

### 後台功能
- ✅ 商品管理 (CRUD)
- ✅ 圖片上傳管理
- ✅ 3D模型上傳
- ✅ 分類標籤管理

---

## 🚀 快速開始

### 環境需求
- Node.js 18+
- MySQL 8.0+
- Vue CLI 5+

### 前端啟動
```bash
cd finall_front
npm install
npm run dev
```

### 後端啟動  
```bash
cd finall_back
npm install
# 配置 .env 環境變數
node app (也可使用 : nodemon app)
```

---

## 💭 開發心得

這個專案是我從零基礎學習程式開發4個月後的成果展現。從最初的 HTML/CSS/JS 3件套基礎，到學習 Vue 3 系列，再到後端 Express 開發，每一步都充滿挑戰。

常常有意想不到的問題，或新的專業知識或插件要學習，往往都是靠自學解決問題與持續開發。

這次專案最大的收穫就是，理解了全端開發的完整流程，以及如何運用 AI 輔助開發來提升效率。

雖然代碼還有優化空間，但功能的完整性讓我對自己的學習成果有相當大的成就感。

---

## ✨ 系統畫面展示

### 🛒 前台購物體驗
<table>
  
  <tr>
     <td width="100%">
      <img src="docs/screenshots/frontend/home_index.png" alt="官網首頁"/>
      <p align="center"><b>官網首頁</b></p>
    </td>
  </tr>
  <tr>
    <td >
      <img src="docs/screenshots/frontend/home_productPage.png" alt="商品頁面"/>
      <p align="center"><b>商品頁面</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/frontend/home_productDetail.png" alt="商品詳情"/>
      <p align="center"><b>商品詳情</b></p>
    </td>
    </tr>
  <tr>
     <td>
      <img src="docs/screenshots/frontend/home_3D.png" alt="3d預覽"/>
      <p align="center"><b>3d預覽</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/frontend/home_productCart.png" alt="購物車"/>
      <p align="center"><b>購物車</b></p>
    </td>
  </tr>
  <tr>
     <td>
      <img src="docs/screenshots/frontend/home_checkout.png" alt="結帳頁面"/>
      <p align="center"><b>結帳頁面</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/frontend/home_checkoutList.png" alt="訂單列表"/>
      <p align="center"><b>訂單列表</b></p>
    </td>
  </tr>
  <tr>
     <td>
      <img src="docs/screenshots/frontend/home_checkoutListContent.png" alt="訂單詳情"/>
      <p align="center"><b>訂單詳情</b></p>
    </td>
  </tr>
</table>

### 🔧 後台管理系統
<table>
  <tr>
    <td width="100%">
      <img src="docs/screenshots/backend/product_productsList.png" alt="產品列表"/>
      <p align="center"><b>產品列表</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/backend/product_editProduct.png" alt="編輯產品"/>
      <p align="center"><b>商品編輯</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/backend/product_tag.png" alt="標籤管理"/>
      <p align="center"><b>標籤管理</b></p>
    </td>
  </tr>
  <tr>
    <td>
      <img src="docs/screenshots/backend/product_cat.png" alt="分類管理"/>
      <p align="center"><b>分類管理</b></p>
    </td>
  </tr>
  
</table>

### 🔐 登入與註冊
<table>
  <tr>
    <td width="50%">
      <img src="docs/screenshots/login/login.png" alt="登入頁面"/>
      <p align="center"><b>登入頁面</b></p>
    </td>
    <td width="50%">
      <img src="docs/screenshots/login/register.png" alt="註冊頁面"/>
      <p align="center"><b>註冊頁面</b></p>
    </td>
  </tr>
</table>

---

<div align="center">

**⭐ 如果這個專案不錯，可以給個 Star 感謝你的鼓勵！**

**📧 聯絡方式**: wayne676803@gmail.com

</div>
