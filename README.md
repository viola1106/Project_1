# 臺北市社會治安-竊盜犯罪分析

### 研究動機
1. 近年社會治安的關注度提高
2. 組員住在台北或在台北就業
3. 瀏覽平台資料時發現臺北市有提供竊案的統計資料，從之瞭解北市各區需要注意的竊案類型

### 資料來源 Data source
[政府開放資料平台](https://data.gov.tw/)      
竊盜犯罪的類型包含 : 住宅竊盜、汽車竊盜、自行車竊盜、機車竊盜、街頭隨機搶奪、街頭隨機強盜等六種案類犯罪。但因為街頭隨機搶奪、街頭隨機強盜，這兩類犯罪類型發生地點不固定，且基於各資保護，提供的資訊略少，因此本次分析不採用。    
資料年份: 2018~2021年
1. 住宅竊盜
2. 汽車竊盜
3. 自行車竊盜
4. 機車竊盜    

[臺北市統計資料庫查詢系統](https://statdb.dbas.gov.taipei/pxweb2007-tp/dialog/statfile9.asp)      
臺北市各類型資料(人文、地理、犯罪...等)，資料可溯及70、80年代，完整性可以再更好。須注意網頁有時候會無法使用。     
1. 警力配置統計資料–2019~2021年
2. 家庭設備(汽、機車)的普及率–2019~2020年

### 資料清理 Data cleaning
* 用Excel統整欄位    
  使用函數: LEFT, RIGHT, MID, CANCAT, VLOOKUP
* 合併檔案
* 統一時間表示方式: 篩選功能手動調整

### 資料視覺化 Data visualization
* 使用[**Tableau**來呈現](https://public.tableau.com/views/-_16498255494290/cover?:language=zh-TW&publish=yes&:display_count=n&:origin=viz_share_link "臺北市社會治安-竊盜犯罪分析")並加以說明。  

地圖呈現2018 ~2021年臺北市各行政區竊案統計     
![地圖](https://user-images.githubusercontent.com/81075616/173486949-2fc44a5d-549e-4bdb-a83a-aac2ffe1655e.png "臺北市行政區竊案統計地圖")
(圖一:地圖)  

請看以下圖片為 "各行政區與案發時間關係圖"
![各行政區與案發時間關係](https://user-images.githubusercontent.com/81075616/173487060-0df8b538-71c4-40c4-b5f6-d6ee1e777d10.png "各行政區與案發時間關係")    
(圖二:各行政區與案發時間關係)    

Tableau可以線上操作，點選想看的竊案類型及行政區，對比一天24小時中最容易發生的時間。  
以自行車為例，案發數最多的是**大安區**，當日時間**早上8 ~10時**的好發率最高。     
![自行車-大安區](https://user-images.githubusercontent.com/81075616/173487188-882e01dc-ef93-4161-861d-09f1b4bd1873.png "自行車-大安區")    
(圖三:自行車-大安區)     

參考下圖可以得出結論:
  * 自行車竊盜案件發生之首在*大安區*
  * 住宅竊盜案件發生之首在*中山區*
  * 汽車竊盜案件發生之首在*北投區、萬華區*
  * 機車竊盜案件發生之首在*萬華區*
![臺北市各行政區4種案件發生次數](https://user-images.githubusercontent.com/81075616/173488900-0d9a3ab5-0cb3-424f-b3de-9d33de08b56e.png "臺北市各行政區4種案件發生次數")    
(圖四:臺北市各行政區4種案件發生次數)  

![家庭設備(汽、機車)的普及率–2019~2020年](https://user-images.githubusercontent.com/81075616/173491943-1ea73b4f-38e1-4bc2-8956-d1a09fce1e16.png "家庭設備(汽、機車)的普及率–2019~2020年")    
(圖五:家庭設備(汽、機車)的普及率–2019 ~2020年)   

![警力配置統計資料–2019~2021年](https://user-images.githubusercontent.com/81075616/173492046-d8cd8ba0-1b39-404e-bca0-1240b9115846.png "警力配置統計資料–2019~2021年")
(圖六:警力配置統計資料–2019 ~2021年)   

同時參考"家庭設備(汽、機車)的普及率–2019~2020年"資料，可以發現，汽機車的普及率與竊盜案發生數呈現正相關。     
由此判斷，除了加強安全宣導之外，也須讓持有者有更高的防竊意識。     
同時警民的協調配合也有待加強，守望相助隊與警察的巡邏時段可以互補，防止竊案發生。    

另外，可以參考下圖圖七發現竊案多發生在1、7、8月，正好是學生們放寒暑假的時候。有學生犯案的疑慮。因個資問題並未取得犯罪者年齡分布，但竊案犯罪年齡層介於學生之間的可能性偏高。
![竊案月份統計](https://user-images.githubusercontent.com/81075616/173489737-d84fbf2a-ed00-4a30-b4b8-b07aac00045c.png "竊案月份統計")     
<img src="https://user-images.githubusercontent.com/81075616/173489737-d84fbf2a-ed00-4a30-b4b8-b07aac00045c.png" width=width="200" height="200" alt="竊案月份統計"/>   
(圖七:竊案月份統計)     

### 結論與價值
從圖二的互動圖表可以得出各行政區號發的竊案及時段，並參考圖五、圖六，可以得出以下結論:
* 依**時間**
  * 多發生在白天
  * 案發率在寒暑假期間明顯偏高
* 依**地區**
  * 萬華區:機車安全
  * 大安區:自行車安全
  * 中山區:住宅安全
* 時間:警民配合&學校家長 
  * 巡邏時間的分配:白天應增加巡邏頻率
  * 學校及家長加強學生品德教育
* 地區:居民自覺
  * 萬華區&大安區居民及工作者須增加對機車&自行車竊案的警覺性
  * 中山區居民應加強確認門窗是否上鎖
* 其他:機車普及率
  * 機車普及率的變化:萬華區移居到內湖區
  * 提供防竊系統公司作為業務行銷的參考依據


#### 由許又元、李悅、王品琪合作完成 Project_1:臺北市社會治安-竊盜犯罪分析    
(更新時間:2022/06/14)
