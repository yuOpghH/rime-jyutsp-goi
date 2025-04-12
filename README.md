# rime-jyutsp_goi
<h1 align="center">jyutsp_goi - 係粵語雙拼+倉頡輔助碼嘅輸入法方案。</h1>

- [1. 致謝](#1-致謝)
- [2. 介紹](#2-介紹)
- [3. 使用方法](#3-使用方法)
- [4. 碼長展示](#4-碼長展示)
- [5. 入門成本](#5-入門成本)
- [6. 文檔說明](#6-文檔說明)
- [7. 常見問答](#7-常見問答)


## 1. 致謝
- 感謝以下項目的無私貢獻及項目成果。
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
係以「香港語言學學會粵語拼音方案」以及「港標字體」為格式嘅粵拼雙拼、喺基礎上加埋倉頡輔助碼的四碼輸入的混撈輸入法。

即全碼四碼：兩碼音碼+倉頡碼。雙拼輸入法經已流行咗好耐，雙拼輸入法將擊鍵數有效壓縮至相對為兩鍵一碼嘅科學打字法。

針對常用嘅書面字、粵字等3000單字及兩萬餘詞、5000餘四字詞作優化，搭載超大詞庫，覆蓋日常打字範圍90%。

（若您在使用途中多有BUG、實為力有所不及，敬請原諒）

# 輸入編碼
## 碼表

[![zhihu]](https://www.zhihu.com/question/54691506/answer/1022245649)

[zhihu]:https://pic2.zhimg.com/80/v2-c7ea6ffcfe550d4bc31ef38a27e5edfd_720w.jpg "碼表"


## 3. 使用方法
- 1，（本體）下載jyutsp_goi.rar，解壓後分別按照文檔存放各處位置覆蓋，然後在輸入法括選併重新部署。（建議備份好原文檔）

- 2，（其他文檔）在部署好本體後，再用補丁覆蓋。預備好“預設簡中”“預設台標繁中”等補丁。擇適用可。

- 3, （手機） 為安撞（android）應用 trime 同文輸入法 適用打字鍵盤主題。放置手機內rime目錄，載入即可。

- 4，（學習文檔）用家可自擇自行下載部署好[極速跟打器](http://www.jsxiaoshi.com/)後，下載極速跟打器.rar按照路徑部署相關檔案，在設置內更換好”編碼文件“。即可使用“練習→字根練習”“發文→文章→繁體常用單字”等相關教程學習。(注：該程序不兼容粵字，練習請用繁體常用單字)


## 4. 碼長展示：
- 各個國家有各個國家嘅國歌
  - 全拼：`gok ge gwok gaa jau gok ge gwok gaa ge gwok g`o（35隻字符）
  - 雙拼：`gp ge xp ga ja gp go xp ga ge xp go`（24隻字符）
- 人皆生而平等，享有造物主賦予給他們的不可剝奪的權利，包括生命、自由和追求幸福的權利
  - 全拼：`jan gaai sang ji ping dang ，hoeng jau zou mat zyu fu jyu kap taa mun dik bat ho mok dyut dik kyun lei，baau kut sang ming、zi jau wo zoei kau hang fuk dik kyun lei`（唔計空格126隻字符）
  - 雙拼：`yf gv sj yi p; dg , ht yb zu mc zy fu yy km ta mr dik bc ho mp dd dik kr lz，bn kt sj m; 、zi yb wo zx kb hg fd dk kr lz`（唔計空格81隻字符）
（以上數據使用work統計）  


### 例：
<p align="center">
<img float=right src="https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E5%B1%95%E7%A4%BA/%E7%B2%B5%E8%AA%9E%E9%9B%99%E6%8B%BC%E5%B1%95%E7%A4%BA.gif"/>
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

繁簡一鍵切換：`Ctrl+Q`

輸出歷史記錄：`aa`

時間日期快捷：`date` `time`

#### 反查

音碼篩選： 思：`si[` 時：`si[[`

倉頡碼：`Q:hwmvs` 粵  

粵語全拼：`W:jyut` 粵

普通拼音：`E:yue` 粵

筆劃反查：`R:丿丨乙丿丶丿一丨丿丶一一乙` 粵

選字6、7、8、9，可用ctrl+1、ctrl+2、ctrl+3、ctrl+4依次對應

## 5. 入門成本
### 學習成本：

用家需先通曉粵拼、改習雙拼鍵打法、倉頡碼噉嘅三重功序：

- 1，粵拼：從零開始，粵人母語者一周到兩周時間大概可通習。
 - 2，雙拼鍵打：從全拼轉雙拼打法，更換鍵盤輸入，大概幾天到一周時間。
  - 3，倉頡碼：從零到熟習，需一周或兩周時間。
  - 
- 若果你係學習過粵拼及倉頡碼，學習成本約一周左右
 - 若果你係學習過倉頡碼，學習成本約兩周左右
  -若果你係從零開始，學習成本約四周左右


#### 優點：
1，平均兩碼出一字

2，常用字有快速碼、優先出簡。可用文檔自行修改順序。

3，針對常用粵字書面字依次做排序。默認以繁體港標為準。

4，加入以詞定字，“，”“。”可從組詞揀字。如輸入：斬纜，撳“]”鍵淨出單字“纜”。

5，音碼非強制，但加倉頡輔助碼可用於更快揀單字

6，五字碼可打長句長詞

7，支持單字音碼揀字（但不組詞），輸入兩碼使用“[”“]”“\”鍵，一下陰兩下陽。

8，支持倉頡碼、粵語全拼、普通拼音、筆劃反查

9，導入大詞庫，打字更輕擎

#### 缺點：
1，學習成本高，用家必須通曉粵拼、雙拼、倉頡。

2，rime自動記詞機制容易錄入奇怪的非常用詞

3，大詞庫項目引用於普語項目，易出非想要詞

4，皆因搭載多個翻譯器。基於兩碼組成嘅長句詞彙大部分可自動錄入(但一部份出於莫名緣故自動錄入機制失效)，五字長句需要在文檔中手動添加

5，四碼輸入，可能固定字碼和組詞衝突，五碼時，揀詞或輸出長詞句衝突

6，超大詞庫，超大冗餘

7，基礎詞庫收音多，因而有使用非常用音字、多音字組詞問題，僅在常用多音字作分詞優化

## 6. 文檔說明
- 用戶文檔/
  - jyutsp_top 文檔：主要為：單字碼、三字碼、以及一些衝突的四字碼。可在此修改優先順序
  
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

- Q 2:點解要用jyutsp方案做雙拼基底
  - A 2:佢係市面家下佔用嘅鍵位最少嘅方案

- Q 3:學習成本咁高點解要用你
  - A 3:的而且確。但目的係想畀一個想用母語輸出又想打得快嘅粵語用家有多一種選擇

- Q 4:點解要加輔助碼，輔助碼點解係倉頡碼。
  - A 4.1:打字唔止話淨出詞，仲要出字，要想打得快又要固定序，添加輔助碼係固定順序又減少記憶嘅折衷方案。
  - A 4.2:倉頡僅120個倉頡字母，學習成本相對較低，且多數港澳學校都有教導。

- Q 5：有啲置頂字詞我唔係好想要喎，點整走佢
  - A 5： 揾到jyutsp_top.txt、jyutsp_zaamsihangci.txt點開，刪又得改後邊嘅數字換序又得。

