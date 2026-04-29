
# 美以伊地緣政治衝突對能源市場之影響分析

本專題利用 Python 進行量化分析，探討戰爭風險對能源市場的結構性影響。

## 專題架構
1. **資料清理**：透過 `yfinance` 獲取數據並處理 MultiIndex。
2. **多維度分析**：涵蓋時間趨勢、市場情緒、跨資產相關性與宏觀溢出效應。
3. **AI 預測**：使用 Prophet 進行時間序列建模。

## 數據分析與可視化 (Dashboard)

### 1. 時間與波動視角
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>油價走勢</b></p> ![油價](images/oil_trend.png) </div>
  <div style="flex: 1;"><p><b>黃金走勢</b></p> ![黃金](images/gold_trend.png) </div>
</div>
<p><b>油價波動率</b> ![波動率](images/volatility.png) </p>

### 2. 情緒與市場動能
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>新聞情緒趨勢</b></p> ![情緒](images/sentiment.png) </div>
  <div style="flex: 1;"><p><b>期貨成交量</b></p> ![成交量](images/volume.png) </div>
</div>

### 3. 資產連動分析
<div style="display: flex; gap: 10px;">
  <div style="flex: 1;"><p><b>油金回歸散點圖</b></p> ![散點圖](images/scatter.png) </div>
  <div style="flex: 1;"><p><b>油金標準化比較</b></p> ![比較](images/compare.png) </div>
</div>
<p><b>股市與油價滯後相關</b> ![相關性](images/lag_corr.png) </p>

### 4. 模型與矩陣
* **相關矩陣**：![矩陣](images/matrix.png)
* **Prophet 價格預測**：![預測](images/forecast.png)

## 結論
戰爭引發的價格跳躍證實了傳統避險邏輯在極端地緣風險下的失效。透過本專題，我們成功驗證了情緒數據與成交量作為預測地緣風險的前瞻指標之價值。

---
**Author**: 數據分析專題小組
**Tools**: Python, Pandas, Matplotlib, Prophet, TextBlob
