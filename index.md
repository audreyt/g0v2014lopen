---
title       : 開放語料運動
subtitle    : Open Corpus Movement
author      : 謝舒凱 (Aber) and Pierre Magistry (A-Tsioh)
job         : 台大語言學研究所助理教授 (2010-)/台大語言學研究所博士後訪問 (2013-2014)
logo        : lopen.jpg
date        : 2014年11月8日
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
url         : {lib: "libraries"}
widgets     : [bootstrap, quiz, shiny, interactive, mathjax]  # {}
ext_widgets : {rCharts: [libraries/widgets/nvd3]}
mode        : selfcontained # {standalone, draft}

---
## 想法 (Two cents)

1. 語言學和開放政府的關係
2. 開放語料的意義與實作架構
3. 開放語料的未來芻議



--- bg:#FFFAF0

## 想法 (Two cents)

1. __`語言學和開放政府的關係`__
2. 開放語料的意義與實作
3. 開放語料的未來芻議


--- .dark .nobackground .quote
# 2 分鐘背景知識
### 2 minutes Linguistics


---
## 語言學是什麼? What is Linguistics ?

- 語言學要回答`語言的習得與發展`，`結構與功能`，`神經與心理機制`，`社會變異與演化過程`等。
- 經驗/計算語言學 (empirical/computational linguistics) [a.k.a. Natural Language Processing] 用電腦來幫助我們回答上述問題，並產生應用。

- (大數據中的) 語言數據（**語料**）蘊含了**文化歷史記憶，社會心理趨勢，政治輿情傾向，情緒偏好分佈，人格特質與決策行為，疾病前期徵兆等等**。 


--- 

## 語言分析與處理是資料科學的第二把刀 Linguistic analysis and Data Science

> - `Linguistic data are ubiqutous`, knowledge to be discovered, tendency to be predicted.

> - 自然語言處理 (Natural Language Processing) and 文本分析技術 (Textual Analytics) are the keys [Why? pressing `p`]

*** =pnotes
<q>
> Enormous amounts of textual information are becoming available electronically on a daily basis,...... Natural Language Processing (NLP) techniques have been playing an increasing role in extracting and managing entities and relations from text... substantially reducing the overhead of the development process.
</q>






---
## 語料是什麼 What are Linguistic Data ?


- 為了溝通與表情（情緒）達意（思維），我們所實現出來的語言資料。

- 在計算語言學（自然語言處理）的脈絡下，廣義的語料包括各項`語言資源`（字典 dictionay，詞庫 lexicon，語料庫 corpus，語法樹庫 treebank，知識本體 ontologies，等等。）




---
## 語言學與零時政府 Linguistics and Open Government

- 之間的距離沒有妳想的那麼遠。
- 數位時代下的多元與巨量趨勢，語料科學對於科學與社會的影響力正在發酵。
- 開發各種語言資訊應用，理解與推展社會進步的潛力

- 政府 >> 公民嗨客(civic hacking) >> 學界 >> 產業
> open the data >> hacking the data >> exploring the data >> data social product






---
## 想法 (Two cents)

1. 語言學和開放政府的關係
2. __`開放語料的意義與實作`__
3. 開放語料的未來芻議






---
## 台語輸入 TaigiIME: A story from A-Tsioh
### 阮若打開 MOE ê Data

> Thanks to MOE's opening of its 《臺灣閩南語常用詞辭典》I could:
- turn a small experiment into an APP
- which was downloaded 10,000 times

### How `TaigIME-android` came into existence

> As a foreign student in linguistics. I noticed that many friends were using Taiwanese (Holo) in there online messages. It was either
- directly in ㄅㄆㄇㄈ
- or in 漢字 using Mandarin sounds in ㄅㄆㄇㄈ as IME...
As a computational linguist, the second option just drove me crazy.
How inconvenient is that !?! 
Can't you just use the transcription of Taiwanese sound to input 漢字 ?!?


---
## 台語輸入 TaigiIME: A story from A-Tsioh

> I had the idea, but was missing the Data.... and MOE.cc found!!
> If the MOE had selected a too restrictive licence, the APP would never had made its way up to the Google Play Store, and now with the status of downloaded more than 10.000 times ! <https://github.com/a-tsioh/TaigIME-android/>

<img class='center'src="assets/img/taigiIME.png" alt="Drawing" style="width: 400px; height：200px"/>



- sadly no pull requests yet
- but quite a lot of feedback for a single man ! (I wish I had more time to spend on it)


---
## Linked Linguistic Data Movement 

[Open Linguistics] (http://linguistics.okfn.org/)

<img class='center'src="assets/img/llod-cloud.png" alt="Drawing" style="width: 500px; height：200px"/>



---
## LOPEN and BIGLEX 

<iframe width="60" height="50" src='assets/img/lopen.png' frameborder="0" allowfullscreen></iframe>





--- .shout #demo

# [DEMO: 開放語料系統](http://lopen.linguistics.ntu.edu.tw/copens) 

<img class='center'src="assets/img/copens.png" alt="Drawing" style="width: 800px; height：250px"/>

---
## BIGLEX ：萌典的學伴（學界版）




--- &interactive

## `BIGLEX`: Exploratory, Reproducible, Scaled

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>require(googleVis)
M1 <- gvisMotionChart(
  Fruits, idvar = 'Fruit',
  timevar = 'Year')
print(M1, tag = 'chart')</textarea>





---
  
## Goals and questions to answer 
  
我們的~~理想~~長遠目標

1. 人人都可以玩（語言）科學，只要她想。
2. 人人都可以邊玩邊練功邊貢獻社會，就算她沒在想。
3. 這可能嗎？
  
<a class="btn btn-large btn-danger" rel="popover" data-content="大家轉念願意放下，理解到知識從來就不應私有化。" data-original-title="" id='example'>很抱歉，不可能。除非</a>
<a id='example' data-content='Change directory doesn't actually change the directory. It changes the shell's idea of which directory we are in' data-original-title='Note'></a>







---
## 立委問政行為: PART I 

<div id = 'chart1' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawchart1()
    });
    function drawchart1(){  
      var opts = {
 "dom": "chart1",
"width":    800,
"height":    400,
"x": "Hair",
"y": "Freq",
"group": "Eye",
"type": "multiBarChart",
"id": "chart1" 
},
        data = [
 {
 "Hair": "Black",
"Eye": "Brown",
"Sex": "Male",
"Freq":             32 
},
{
 "Hair": "Brown",
"Eye": "Brown",
"Sex": "Male",
"Freq":             53 
},
{
 "Hair": "Red",
"Eye": "Brown",
"Sex": "Male",
"Freq":             10 
},
{
 "Hair": "Blond",
"Eye": "Brown",
"Sex": "Male",
"Freq":              3 
},
{
 "Hair": "Black",
"Eye": "Blue",
"Sex": "Male",
"Freq":             11 
},
{
 "Hair": "Brown",
"Eye": "Blue",
"Sex": "Male",
"Freq":             50 
},
{
 "Hair": "Red",
"Eye": "Blue",
"Sex": "Male",
"Freq":             10 
},
{
 "Hair": "Blond",
"Eye": "Blue",
"Sex": "Male",
"Freq":             30 
},
{
 "Hair": "Black",
"Eye": "Hazel",
"Sex": "Male",
"Freq":             10 
},
{
 "Hair": "Brown",
"Eye": "Hazel",
"Sex": "Male",
"Freq":             25 
},
{
 "Hair": "Red",
"Eye": "Hazel",
"Sex": "Male",
"Freq":              7 
},
{
 "Hair": "Blond",
"Eye": "Hazel",
"Sex": "Male",
"Freq":              5 
},
{
 "Hair": "Black",
"Eye": "Green",
"Sex": "Male",
"Freq":              3 
},
{
 "Hair": "Brown",
"Eye": "Green",
"Sex": "Male",
"Freq":             15 
},
{
 "Hair": "Red",
"Eye": "Green",
"Sex": "Male",
"Freq":              7 
},
{
 "Hair": "Blond",
"Eye": "Green",
"Sex": "Male",
"Freq":              8 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        
          
        

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

---
## 表格數據與文本數據 Structured and un-structured data

> "脫黨投票不一定較好，可能該立委是憑良心投票，也可能是受財團、企業影響所致，還請點選該立委觀看其脫黨投票的表決**內容**再作論定。"

> "量化數據不能代表好壞只能參考，修正草案數多不一定較好，還請點選該立委觀看其修正草案的**內容**再作論定。" <http://ly.g0v.tw/>





--- 
## 立委問政行為: PART II


<div class="row-fluid">
  <div class="span4">
    <form class="well">
      <label class="control-label" for="sex">Choose Sex</label>
      <select id="sex"><option value="Male" selected>Male</option>
<option value="Female">Female</option></select>
      <script type="application/json" data-for="sex" data-nonempty="">{}</script>
      <label class="control-label" for="type">Choose Type</label>
      <select id="type"><option value="multiBarChart" selected>multiBarChart</option>
<option value="multiBarHorizontalChart">multiBarHorizontalChart</option></select>
      <script type="application/json" data-for="type" data-nonempty="">{}</script>
    </form>
  </div>
  <div class="span8">
    <div id="nvd3plot" class="shiny-html-output nvd3 rChart"></div>
  </div>
</div>







---
## 立委問政行為: PART III

> 國會測謊器：文本，論述，表情與政治 （無誠勿入）

<iframe width="60" height="50" src='assets/img/microexpressions-lie-to-me.jpg' frameborder="0" allowfullscreen></iframe>




--- bg:#FFFAF0

## 想法 (Two cents)

1. 語言學和開放政府的關係
2. 開放語料的意義與實作
3. __`開放語料的未來芻議`__


---
## 從「還文於民」到「還語於民」

* 原視，公視，客語台影音文稿。
* 中央通訊社新聞。
* 各式公文宣導手冊。
* (以 NPR API 為例)


---
## 給出愈多，得到愈多

### 從基本詞彙到台灣南島語言族譜 (Austronesian linguistic phylogenetics)


<img class='center'src="assets/img/formosan.png" alt="Drawing" style="width: 500px; height：200px"/>


---
## 萌典學界版 

* 從詞典(dictionary) 詞庫 (lexicon) 詞網 (lex.network) 詞雲 (lex.cloud)

<img class='center'src="assets/img/cwm.png" alt="Drawing" style="width: 450px; height：150px"/>



---
## 結論：信願行 Conclusion


* <img class='center'src="assets/img/hacker.png" alt="Drawing" style="width: 350px; height：150px"/>

* Bridge the gap between the labs and the people !

* 眾籌眾包眾什麼都歡迎 Crowd (found|sourc)ing language resources for Taiwan.


---
# 謝謝大家！

- Slides: <http://loperntu.github.io/g0v2014lopen/>
- LOPEN project: <http://bit.ly/4lopen> 請幫忙！




