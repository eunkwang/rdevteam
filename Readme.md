Install
-------

    devtools::install_github("lovetoken/rdevteam")
    library(rdevteam)

<br><br>

주요기능
--------

### 네이버 연관검색어 추출 : `naverRelation1()`, `naverRelation2()`

    ex1 <- naverRelation1("한국")
    ex2 <- naverRelation2("한국")

    ex1

    ##  [1] "미국"          "일본"          "북한"          "러시아"       
    ##  [5] "영국"          "인도"          "대만"          "독일"         
    ##  [9] "캐나다"        "프랑스"        "세계 GDP 순위" "베트남"       
    ## [13] "호주"          "한국 축구"     "태국"          "한국 한자"    
    ## [17] "gdp"           "스페인"        "남한"          "스위스"

    ex2

    ## # A tibble: 380 x 2
    ##    R1    R2      
    ##    <chr> <fctr>  
    ##  1 미국  대한민국
    ##  2 미국  러시아  
    ##  3 미국  한국    
    ##  4 미국  인도    
    ##  5 미국  캐나다  
    ##  6 미국  영국    
    ##  7 미국  프랑스  
    ##  8 미국  독일    
    ##  9 미국  호주    
    ## 10 미국  브라질  
    ## # ... with 370 more rows

    library(networkD3)

    simpleNetwork(ex2)
    networkplot_3d(ex2)

<br>

### 네트워크 시각화 : `nvrGraph()`

    nvrGraph("사과")

<br><br>

License
-------

[GPL-3](https://www.gnu.org/licenses/gpl-3.0.en.html)
