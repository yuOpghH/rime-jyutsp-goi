# rime-jyutsp_goi 

<h1 align="center">jyutsp_goi - 基於rime嘅粵語雙拼+倉頡輔助碼輸入法方案</h1>

<h1 align="center">
 
<p align="center"><a href="https://github.com/yuOpghH/rime-jyutsp_goi/releases"><img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/download-button.jpg" style="width: 150px;"/></a></p>

</h1>



- [1. 致謝](#1-致謝)
- [2. 介紹](#2-介紹)
- [3. 使用方法](#3-使用方法)
- [4. 碼長展示](#4-碼長展示)
- [5. 入門成本](#5-入門成本)
- [6. 文檔說明](#6-文檔說明)
- [7. 常見問答](#7-常見問答)
- [8. 其他圖片展示](#8-其他圖片展示)


## 1. 致謝
- 感謝以下項目的無私貢獻及項目成果。可能有遺漏敬請原諒。
 - 鍵盤設置來源 [jyutsp粵語雙拼](https://github.com/MrCorn0-0/jyutsp/)

 - 詞庫增強來源 [Rime 詞庫增強](https://github.com/Iorest/rime-dict/)

 - 音碼基底來源 [貍貓粵拼](https://github.com/leimaau/leimaau_jyutping/)

 - 詞庫基底來源 [Rime 粵語拼音方案](https://github.com/rime/rime-cantonese/)

 - 依賴反查：[倉頡5代](https://github.com/rime/rime-cangjie/)

 - 依賴反查：[Rime 粵語拼音方案](https://github.com/rime/rime-cantonese/)

 - 依賴反查：[明月拼音](https://github.com/rime/rime-luna-pinyin/)

 - 依賴反查：[筆劃](https://github.com/rime/rime-stroke/)

 - lua功能：[以詞定字](https://github.com/BlindingDark/rime-lua-select-character)

 - 字詞優先順序語料來源：[粵典](https://words.hk/)

## 2. 介紹

<h1 align="center">粵拼雙拼改 jyutsp_goi 輸入法。</h1>

jyutsp_goi輸入法 
本方案係依賴於[Rime](https://rime.im/)以「香港語言學學會粵語拼音方案」以及「港標字體」為格式嘅粵拼雙拼方案、喺基礎上加埋倉頡輔助碼的四碼輸入的混撈輸入法。

即全碼四碼：兩碼音碼+倉頡碼 的音形碼（形碼可忽略、可只打音碼）。雙拼輸入法經已流行咗好耐，雙拼輸入法將擊鍵數有效壓縮至相對為兩鍵一碼嘅科學打字法。

針對常用嘅書面字、粵字等3500單字及兩萬餘詞、5000餘四字詞作優化，3000字內重碼率為5.8%，3500字內為7.8%，上下浮動6~8%之間（通過極速賽碼器統計），搭載超大詞庫，覆蓋日常打字範圍95%+。

（若您在使用途中多有BUG、實為力有所不及，敬請原諒）

----
- 更新日誌：
  - 版本 2025-05-01 update：重新梳理3500字的固定簡碼，引入新嘅翻譯器解決custom_phrase造詞阻擋問題。導入新lua “is_in_user”提示造詞上屏記錄、使用rimetool引用新輸入法陰影主題。
  - 版本 2025-05-14 update：從現在開始提供“完全安裝”版本，無有rime的用家可以通過“完全安裝”程式包直接一步佈置好。

</br>（注意！由於更新反查方案的緣故，首次使用時，所以請至少在方案選單設定中載入方案“jyutsp_faancaa（粵語雙拼 反查雙拼+全拼）”一次，其後可取消，否則無有返查）
# 輸入編碼
## 碼表

[![zhihu]](https://www.zhihu.com/question/54691506/answer/1022245649)

[zhihu]:https://pic2.zhimg.com/80/v2-c7ea6ffcfe550d4bc31ef38a27e5edfd_720w.jpg "碼表"


## 3. 使用方法
- 1，（本體）
  - 1.1 （未曾擁有rime，pc端），請下載 weasel-with-jyutsp_goi X.X-installer（完全安裝）版，直接安裝，等待程式佈置完成即可使用。
  - 1.2 （已擁有rime，或其他端rime），請下載jyutsp_goi 20XX-XX-XX.rar（僅方案），解壓後分別按照文檔存放，右鍵系統托盤的Rime圖標選擇“用户文件夾”“程序文件夾”等對應各處位置覆蓋，然後在輸入法選中併重新部署。（建議備份好原文檔）
</br>（首次使用時，所以請至少在方案選單設定中載入方案“jyutsp_faancaa（粵語雙拼 反查雙拼+全拼）”一次，其後可取消，否則無有返查）

- 2，（其他文檔）在部署好本體後，再用補丁覆蓋。預備好“預設簡中”“預設台標繁中”等補丁。擇適用可。

- 3, （手機） 為安撞（android）應用 trime 同文輸入法 適用打字鍵盤主題。放置手機內rime目錄，載入即可。

- 4，（學習文檔）
  - 4.1 此法適合從零開始用家。配置文檔兼有雙拼鍵位、倉頡字根學習練習，用家可自擇自行下載部署好[極速跟打器](http://www.jsxiaoshi.com/)後，下載極速跟打器.rar按照路徑部署相關檔案，在設置內更換好”編碼文件“。即可使用“練習→字根練習”“發文→文章→繁體常用單字”等相關教程學習。(注：該程序不兼容粵字，練習請用繁體常用單字)
  - 4.2 此法適合有基礎用家。無需安裝程式線上使用。用家可打開雲端 [木易跟打器](https://typer.owenyang.top/) ，然後[學習資料](https://github.com/yuOpghH/rime-jyutsp_goi/tree/main/%E6%9C%A8%E6%98%93%E8%B7%9F%E6%89%93%E5%99%A8) 資料夾內的資料配置進去，將 “jyutspgoi 3500字粵音常用字試驗方案.txt”文本拖進 功能/設置/碼表設置中保存，在同頁面打開“編碼提示”，然後在“跟打”複製貼上“粵音常用字%203500字順序.txt”，即可練習。

## 4. 碼長展示：
- 各個國家有各個國家嘅國歌
  - 全拼：`gok go gwok gaa jau gok go gwok gaa ge gwok go`（35隻字符）
  - 雙拼：`gp ge xp ga ja gp go xp ga ge xp go`（24隻字符）
- 人皆生而平等，享有造物主賦予給他們的不可剝奪的權利，包括生命、自由和追求幸福的權利
  - 全拼：`jan gaai sang ji ping dang ，hoeng jau zou mat zyu fu jyu kap taa mun dik bat ho mok dyut dik kyun lei，baau kut sang ming、zi jau wo zoei kau hang fuk dik kyun lei`（唔計空格126隻字符）
  - 雙拼：`yf gv sj yi p; dg , ht yb zu mc zy fu yy km ta mr dik bc ho mp dd dik kr lz，bn kt sj m; 、zi yb wo zx kb hg fd dk kr lz`（唔計空格81隻字符）
（以上數據使用work統計）  


### 例：

<p align="center">
<img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/%E7%B2%B5%E8%AA%9E%E9%9B%99%E6%8B%BC%E5%B1%95%E7%A4%BA%20(1).gif"  style="width:380px;"/>
<img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/%E7%B2%B5%E8%AA%9E%E9%9B%99%E6%8B%BC%E5%B1%95%E7%A4%BA-(2).gif"  style="width:380px;"/>
<img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/%E7%B2%B5%E8%AA%9E%E9%9B%99%E6%8B%BC%E5%B1%95%E7%A4%BA%20(3).jpg"/>
</p>
 
- 一字固定快碼：
  - 我 `u` 你 `n` 愛 `i` 佢 `k`

- 兩字固定字碼：
  - 時 `si` 冚 `kg` 狂 `qw` 

- 三字四字 音碼搭倉頡快速揀字：
  -  知 `zi+o(人) ` 曉 `hq+a（日）` 諗 `ng+y（卜） `
  - 跣 `sn+ru（口山）` 喐 `yd+rl（口中）`

- 四字出固定雙字詞：
   - 知道 `zidu` 𠸎褦 `lang` 𠮩𠹌 `lqng`

- 雙字詞可+一或兩倉頡碼揀詞：
   - 不止 `bczi+y(卜) ` 八字 `bczi+j（十）`  不治 `bczi+e(水)`
 - 亦：
    - 知能 `zi+o(人)+ng` 智能 `zi+oa(人日)+ng`

-  五字出長詞：
   - 吖吱吖咗 `ezez+r(口)` 崩口人忌崩口碗 `bhyw+m(一)`
(括號內係倉頡碼)

### 其他功能展示：

造詞：應輸出全碼使次翻譯器生效，如輸出“`記淥`” ，應打`gzyu（記）+~號+ldee（淥）+~號`，即可上屏記錄，參照項目頭部動態圖片(2)。（關於造詞規則詳細參見[7. 常見問答](#7-常見問答)）

刪詞：使用`ctrl+del`刪除已上屏的詞彙

調整自帶固定字詞序：參見[7. 常見問答](#7-常見問答)，修改jyutsp_top.txt  jyutsp_zaamsihangci.txt即可。

提示功能：通過lua 文字編碼區會提示，”📌“為固定字詞、“🖊️”為當前輸入即上屏(造詞)，”📖“為已鍵入過有歷史記錄的字詞

繁簡一鍵切換：`Ctrl+Q`

輸出歷史記錄：`aa`

時間日期快捷：`date` `time`

以詞定字：“`,`”“`.`”從組詞揀字。如輸出“斬纜”，撳“`,`”鍵淨出單字“斬”，撳“`.`”鍵淨出單字“纜”。

選字6、7、8、9，可用ctrl+1、ctrl+2、ctrl+3、ctrl+4依次對應
#### 反查

音碼篩選： 思 si1：`si[` 時 si4：`si[[`

倉頡碼：`Q:hwmvs` 粵  

粵語全拼：`W:jyut` 粵

普通拼音：`E:yue` 粵

筆劃反查：`R:丿丨乙丿丶丿一丨丿丶一一乙` 粵

## 5. 入門成本
### 學習成本：

用家需先通曉粵拼、改習雙拼鍵打法、倉頡碼噉嘅三重功序：

- 1，粵拼：從零開始，粵人母語者一周到兩周時間大概可通習。
 - 2，雙拼鍵打：從全拼轉雙拼打法，更換鍵盤輸入，大概幾天到一周時間。
  - 3，倉頡碼：從零到熟習，需一周或兩周時間。 


- 若果你係學習過粵拼及倉頡碼，學習成本約一周左右
  - 若果你係學習過倉頡碼，學習成本約兩周左右
    - 若果你係從零開始，僅學習 雙拼鍵打，學習成本約三周左右
      - 若果你係從零開始，並學習 倉頡碼，學習成本約四周左右

(該項目有提供學習文檔，或能提高速度)

#### 優點：
1，平均兩碼出一字

2，常用字有快速碼、優先出簡。可用文檔自行修改順序。

3，針對常用粵字書面字依次做排序。默認以繁體港標為準。

4，加入以詞定字，“,”“.”可從組詞輸出中揀字。如輸入：斬纜，撳“,”鍵淨出單字“斬”，撳“.”鍵淨出單字“纜”。

5，可輸音碼不輸形碼。形碼非強制，但加倉頡輔助碼可用於更快揀單字，也可搭配“以詞定字”揀字。

6，五字碼可打長句長詞

7，支持單字音碼揀字（但不組詞），輸入兩碼使用“[”“]”“\”鍵，一下陰兩下陽。

8，支持倉頡碼、粵語全拼、普通拼音、筆劃反查

9，導入大詞庫，打字更輕擎

#### 缺點：
1，學習成本高，用家必須通曉粵拼、雙拼、倉頡。

2，rime自動記詞機制容易錄入奇怪的非常用詞、<s>組詞自動記憶bug</s>

3，大詞庫項目引用於普語項目，易出非想要詞

4，皆因搭載多個翻譯器。基於兩碼組成嘅長句詞彙大部分可自動錄入(但一部份出於莫名緣故自動錄入機制失效)，五字長句需要在文檔中手動添加

5，四碼輸入，可能固定字碼和組詞衝突，五碼時，揀詞或輸出長詞句衝突

6，超大詞庫，超大冗餘

7，基礎詞庫收音多，因而有使用非常用音字、多音字組詞嘅bug，僅在常用多音字作分詞優化

## 6. 文檔說明
- 用戶文檔/
  - jyutsp_top 文檔：主要為：單字碼、三字碼、以及一啲衝突嘅四字碼。可在此修改優先順序
  
  - jyutsp_zaamsihangci 文檔：主要為：雙字詞彙、多字詞詞碼。可在此修改優先順序
    
  - forjyut.jyut.dict.yaml：粵文詞彙(新詞彙添加此、可用於打長詞翻譯器)
    
  - forjyut.jyutsp.dict.yaml：粵文詞彙。量詞、四鍵長詞可在此修改。
    
  - forjyut.chat.dict.yaml：書面語、普語詞彙
    
  - forjyut.chatcust.dict.yaml：書面語、普語詞彙(新詞彙添加此、可用於打長詞翻譯器)

  - jyutsp_top.txt：置頂多數單字、及部份詞嘅文檔。可修改此更改優先順序。

  - jyutsp_zaamsihangci.txt：置頂多數詞語嘅文檔。置頂多數單字、及部份詞嘅文檔。可修改此更改優先順序。

## 7. 常見問答：

- Q 1：如何修改預設輸出簡體中文/台標繁中
  - <s>A 1：請點開jyutsp_goi.schema.yaml，揾到“字形 → 大陸”呢行，喺上邊嘅“reset: 2"改成”reset: 0“，保存並重新部署。你都可以用“ctrl+Q”快速切換。</s>
  - 使用其他文檔內的補丁即可。

- Q 2:為何要用jyutsp方案做雙拼基底
  - A 2:佢係市面家下佔用嘅鍵位最少嘅方案

- Q 3:學習成本咁高，為何要用你
  - A 3:的而且確。但目的係想畀一個想用母語輸出又想打得快嘅粵語用家有多一種選擇

- Q 4:為何要加輔助碼，輔助碼為何係倉頡碼。
  - A 4.1:打字不單止話淨出詞，仲要出字，要想打得快又要固定序，添加輔助碼係固定順序又減少記憶嘅折衷方案。
  - A 4.2:倉頡僅120個倉頡字母，學習成本相對較低，且多數港澳學校都有教導。

- Q 5:個別置頂字詞非我想要喎，如何修改
  - A 5:揾到jyutsp_top.txt、jyutsp_zaamsihangci.txt點開，刪又得改後邊嘅數字換序又得。

- Q 6：關於造詞規則的詳細
  - A 6：為何組詞規則如此麻煩？
  - 原理：簡而言之，關於rime的造詞優先，custom_phrase（固頂字詞）並不會參與翻譯器如abc、fixed、fixed之間的組詞，這樣會導致混輸入造詞失敗，為此我添加了fixed、fixed2兩個翻譯器進行特別覆蓋。之所以這樣選擇，純用翻譯器對字詞序調整是很麻煩的。
  - 一般來講，對此機制不明，超過3個單字組成的詞彙上屏便能成自造詞，但是這逐一逐一選字，最後一個單字會被固頂覆蓋，從而組詞失敗。
  - 即係，“zihu ~ zuyr ~ ciyr〔造詞中〕”如此輸入一般能上屏，但係輸入“自造ciyr+ ~〔造詞中〕”已上屏前面單字到最後一個時，會導致組詞失敗
  - 即係輸出 “zihu ~ zuyr ~ ciyr〔造詞中〕”仍然有效，所以為了規避特殊（單字上屏）情況，啫係話“唔使用户諗噉多”“嘩太複雜喇”，說明板直接將造詞規則闡明為 “單字之間用`號分隔，然後在結尾多打一個“ ~ ”號就可以嘞。”
  - 即 “zihu ~ zuyr ~ ciyr`~`〔造詞中〕”

## 8. 其他圖片展示

<p align="center">
 <img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/展示/trime.jpg" style="width: 400px;"/>
 </br>
 <img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/learn%2001.png" style="width: 400px;"/>
 </br>
 <img src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/learn%2002.jpg" style="width: 400px;"/>
</p>
