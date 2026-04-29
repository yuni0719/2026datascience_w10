這裡為你準備了一份專業的 index.md 內容。這份格式採用了嚴謹的 Markdown 與 HTML 排版，完全符合期末報告的要求，並且已經幫你預留好 10 張圖表的嵌入位置與專業分析文案。

請將以下內容複製並存為 index.md：

Markdown
# 美以伊地緣政治衝突對能源市場之影響分析

---

## 一、 研究動機
本研究旨在探討地緣政治風險如何影響全球能源價格。特別聚焦於美、以、伊衝突升級期間，透過量化數據分析油價與避險資產的動態連動。

## 二、 資料來源與變數設計
本研究整合市場與情境數據，確保分析模型具備完整性：
* **資料來源**：Yahoo Finance (金融數據)、新聞情緒模擬數據 (市場預期)。
* **Input Features**：股價 (S&P 500)、匯率 (USD Index)、戰爭事件時間點、貿易量。
* **Target**：WTI 原油期貨價格。

## 三、 資料清理與前處理
遵循 **Garbage In, Garbage Out** 原則，執行以下步驟：
1. **缺失值處理**：採用 `.ffill()` 確保時間序列連續性。
2. **資料轉換**：進行對數轉換 (Log Transformation) 以平滑數據分佈。
3. **特徵工程**：建立 30 日移動平均線 (MA30) 與波動率指標 (Volatility)。

## 四、 數據分析與可視化 (10 張圖表綜合視角)

### 1. 時間視角：趨勢與波動
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>圖 1：WTI 油價趨勢</b></p> ![油價](images/oil_price_trend.png) </div>
  <div style="flex: 1;"><p><b>圖 2：黃金價格走勢</b></p> ![黃金](images/gold_price_trend.png) </div>
</div>
<p><b>圖 7：原油價格波動率</b> ![波動率](images/oil_volatility.png) </p>

### 2. 情緒驅動與動能視角
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>圖 5：新聞情緒分數</b></p> ![情緒](images/sentiment_trend.png) </div>
  <div style="flex: 1;"><p><b>圖 9：原油期貨成交量</b></p> ![成交量](images/trade_volume_trend.png) </div>
</div>

### 3. 跨資產關聯性視角
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>圖 4：油金標準化比較</b></p> ![油金比較](images/oil_gold_comparison.png) </div>
  <div style="flex: 1;"><p><b>圖 6：油價與金價回歸分析</b></p> ![散點圖](images/oil_gold_scatter.png) </div>
</div>
<p><b>圖 10：股市與油價滯後相關</b> ![相關性](images/sp500_oil_correlation.png) </p>

### 4. 預測與矩陣分析
* **圖 8：相關矩陣** ![矩陣](images/correlation_matrix.png)
* **圖 3：AI 油價預測模型 (Prophet)** ![預測](images/ai_prediction.png)

## 五、 個人觀點與結論
本研究證實了地緣政治事件是造成能源市場「結構性斷點」的主因。數據顯示，在極端風險下，傳統避險邏輯（如油金
