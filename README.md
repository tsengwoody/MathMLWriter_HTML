## 目標
製作一個給視障者使用的數學編輯器

## 預計使用技術
- Vue.js
- MathJax
- Mathquill

## 參考資料
- [目前實作參考](https://www.edocumentservice.org/ebookSystem/mathml)
- [NVDA語音閱讀器](https://www.nvaccess.org/)
- [社團法人台北市視障者家長協會](https://www.forblind.org.tw/)
- [雲端千眼](https://www.edocumentservice.org/)

## 運算元
A. 上下標、下標、上標
B. 正上下標、正下標、正上標
C. 平方根、多次根
D. 極限、微分、積分
E. 矩陣、行列式、絕對值

## 編輯器
實作分成三個部分
1. 如何製作網頁運算計算器
2. 產生 MathML
3. 切換輸入模式與閱讀模式

## 問題
1. mathjax 可以用閱讀器讀嗎？
2. MathML 的語法結構複雜，使用 Latex to MathML 較合適。
3. 如何將 Latex 轉成 MathML 
4. 如何聚焦唸出現在的式子

12/21
1. 要有一個 data 的結構去 render UI，格式要是 json，因為大部分的動態處理都用 json 互動。
2. 後端丟 mathML 存也是用 mathML 存，用 textarea 存取。
3. 變成前端要做這層處理，處理 mathmltojson 跟 jsontomathml。
4. 純打字的行為用 latex 是好處理的。

## 參考資料
1. [Mathquill 文件](http://docs.mathquill.com/en/latest/Getting_Started/)
2. [JMEditor](http://www.jmeditor.com/)
