# Markdown Cheat List

<!--數學算式語法-->
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({ tex2jax: {inlineMath: [['$', '$']]}, messageStyle: "none" });
</script>
<!-- -->

:::    success
以下內容會以 Markdown 語法的各種功能為主題，只秀出其表示語法以及結果，基本上不會有解釋。

:::    info
Example\:
```markdown=
## example of representation
<font color="red">Hakuna Matata</font>
:)
```
> ## example of representation
> <font color="red">Hakuna Matata</font>
> :)
:::

**Reference**: 
1. [Markdown 常用語法示例 (含Mathjax) - HackMD](https://hackmd.io/@Victor-Zhou/Md%E7%A4%BA%E4%BE%8B)  
2. [HackMD 使用教學 - HackMD](https://hackmd.io/c/tutorials-tw/%2Fs%2Ftutorials-tw)  
3. [Markdown Extention - VSCode](https://code.visualstudio.com/api/extension-guides/markdown-extension)

**沒寫的內容**：<HTML>語法(因為不是這文的重點，會變成<HTML>的教學)、Code(單純我懶 :P)。  
    
---
    
### 標題
```markdown=
# 一級標題(最大)
## 二級標題
### 三級標題
#### 四級標題
##### 五級標題
###### 六級標題(最小)
```
> # 一級標題(最大)
> ## 二級標題
> ### 三級標題
> #### 四級標題
> ##### 五級標題
> ###### 六級標題(最小)

---

### 內文效果
```markdown=
一般內文 Text
**粗體效果** 和 *斜體效果* 可 ***疊加使用***
~~刪除文字~~
==聚光文字==
<small> 小型文字 </small>
<sup>上底</sup>文字
<sub>下底</sub>文字
```
> 一般內文 Text
> **粗體效果** 和 *斜體效果* 可 ***疊加使用***
> ~~刪除文字~~
> ==聚光文字==
> <small>小型文字 (我也不知道為啥前面會出現"----")</small>
> <sup>上底</sup>文字
> <sub>下底</sub>文字

---

### 跳脫字元

```=
\*literal asterisks\*
\- DASH ------ \--\--\-- \-\-\-\-\-\-
\\\\
```
> \*literal asterisks\*
> \- DASH ------ \--\--\-- \-\-\-\-\-\-
> \\\\

::: success
Markdown支援在下面這些符號前面加上反斜線來幫助插入普通的符號：
> ```
> \   反斜線
> `   反引號
> *   星號
> _   底線
> {}  大括號
> []  方括號
> ()  括號
> #   井字號
> +   加號
> -   減號
> .   英文句點
> !   驚嘆號
> ```
:::
    
---

### 無序清單
```markdown=
* 無序清單1
* 無序清單2
    * 無序子清單
        * 無序子子清單
```
> * 無序清單1
> * 無序清單2
>     * 無序子清單
>         * 無序子子清單

---

### 有序清單
```markdown=
1. 有序清單1
2. 有序清單2
    1. 有序子清單
3. 有序清單3
```
> 1. 有序清單1
> 2. 有序清單2
>     1. 有序子清單
> 3. 有序清單3

---
    
### 引文
```=
> 第一層引文
>> 第二層引文
>>> 第三層引文
>>>> 第四層引文
```

> > 第一層引文
> >> 第二層引文
> >>> 第三層引文
> >>>> 第四層引文

---
    
### 註解
```markdown=
<!-- 註解文字 -->
<!-- 註解文字
     註解文字 -->
```
> ::: warning
> :warning: 因為是註解，因此不會看到任何東西
> :::
<!-- 註解文字 -->
<!-- 註解文字
     註解文字 -->
---
    
### Callout有色區塊
```markdown=
:::    success
Success 內文
:::

:::    warning
Warning內文
:::

:::    info
Info 內文
:::

:::    danger
Danger 內文
:::
```
    
> :::    success
> Success 內文
> :::
> 
> :::    warning
> Warning內文
> :::
> 
> :::    info
> Info 內文
> :::
> 
> :::    danger
> Danger 內文
> :::
:::    warning
:warning: 注意： VSCode 並不支援 Callout 功能，使用時應當注意，避免出錯
:::
    
---
    
### Toggle
```markdown=
:::    spoiler 目錄
Toggle Spoiler 收起項目1
Toggle Spoiler 收起項目2
:::

## 或著也可以使用<HTML>來寫
    
<details>
<summary>目錄</summary>

Toggle Spoiler 收起項目1
Toggle Spoiler 收起項目2 

</details>
```
> <details>
> <summary>目錄</summary>
> 
> Toggle Spoiler 收起項目1
> Toggle Spoiler 收起項目2 
> 
> </details>

---

### 勾選選項
```markdown=
哪件事最痛苦？
- [X] 架環境
- [ ] 腦內沒想法
- [ ] 過年時的親戚
```
> - [X] 架環境
> - [ ] 腦內沒想法
> - [ ] 過年時的親戚
    
---

### 相片or超連結
#### 相片
```markdown=
![圖片註記文字](檔名.png "圖名")

## 或著你也可以用<<HTML>>格式表達，而且可以做得更客製化

<img src=https://hackmd.io/_uploads/SkHZJOh6a.jpg alt="shark" title="shhhhark" height="200px" width="200px">
```
> <img src=https://hackmd.io/_uploads/SkHZJOh6a.jpg alt="shark" title="shhhhark" height="200px" width="200px">

---
    
#### 超連結

```markdown=
[超連結標題(喔對了，記得開聲音^^)](https://www.instagram.com/reel/C0Nr1NSs-jO/?utm_source=ig_web_copy_link)
```
> [超連結標題(喔對了，記得開聲音^^)](https://www.instagram.com/reel/C0Nr1NSs-jO/?utm_source=ig_web_copy_link)
    
---
    
### 分隔
```markdown=
以下為分隔線
    
---
    
分隔線結束
```

> <p>以下為分隔線</p>
>
> ---
> 分隔線結束

---

### 數學運算符

```=
在檢視矩陣 $A$ 時，是以 $A^{m}_{n}$ 表示，還是以 $a_{m, n}$ 表示，還是以 $a^{m, n}$ 表示？
```
> 在檢視矩陣 $A$ 時，是以 $a^{m}_{n}$ 表示，還是以 $a_{m, n}$ 表示，還是以 $a^{m, n}$ 表示？

::: info
##### 基本運算符
| MathJax語法 | 對應輸出 | | MathJax語法 | 對應輸出 |
|:----------:|:-------:|:-:|:--------:|:-------:|
| \times | $\times$ | | \div$   | $\div$    |
| \pm    | $\pm$    | | \mp     | $\mp$     |
| =      | $=$      | | \equiv  | $\equiv$  |
| \ne    | $\ne$    | | \approx | $\approx$ |
| \geq   | $\geq$   | | \leq    | $\leq$    |
| \gg    | $\gg$    | | \ll     | $\ll$     |
| \cdot  | $\cdot$  | | \cdots  | $\cdots$  |

##### 邏輯推演：
| MathJax語法 | 對應輸出 | | MathJax語法 | 對應輸出 |
|:----------:|:-------:|:-:|:--------:|:-------:|
| \forall  | $\forall$  | | \exists | $\exists$ |
| \because | $\because$ | | therefore | $\therefore$ |
| \implies | $\implies$ | | iff       | $\iff$  |
| \left( \right)   | $\left(🤔\right)$ | | \left[ \right] | $\left[🤔\right]$ |
| <font color=red>**\left< \right>** | $\left<🤔 \right>$ | | <font color=red>**\{\}<** | $\{🤔\}$ |

     
##### 特殊字符、字母
| MathJax語法 | 對應輸出 | | MathJax語法 | 對應輸出 |
|:----------:|:-------:|:-:|:--------:|:-------:|
| \gamma | $\gamma$ | | \Gamma   | $\Gamma$ |
| \delta | $\delta$ | | \Delta   | $\Delta$ |
| \prime | $\prime$ | | \hat {i} | $\hat {i}$
| \nabla | $\nabla$ | | \circ    | $\circ$  |

##### 其他：
    
```=
$$ \frac{1}{n+4} $$$$
\sum_{i=1}^{n} Time_i $$$$ 
\lim_{x\to\infty} \frac{1}{x} = 0 $$$$ 
\sqrt{2} \approx 1.414 $$

矩陣：
$$ \quad \begin{vmatrix} 1 & 2 \\ 3 & 4 \\ \end{vmatrix} $$
向量:
$$ \vec{r} = \left< Q,R \right> $$
```
    
    
> $$ \frac{1}{n+4} $$$$
> \sqrt{2} \approx 1.414 $$$$
> \sum_{i=1}^{n} Time_i $$$$ 
> \lim_{x\to\infty} \frac{1}{x} = 0 $$$$ 
> \left. \frac{dy}{dx} \right| _{x=0} = f^\prime(0)
> $$$$
> \frac{\partial x}{\partial y}
> $$$$
> \int_1^\infty (p\times{\ln(p)}) dp
> $$
> 
> 矩陣：
> $$ \quad \begin{vmatrix} 1 & 2 \\ 3 & 4 \\ \end{vmatrix} $$
> 向量:
> $$ \vec{r} = \left< Q,R \right> $$
    
[**更多有關LaTEX的數學式 <i class="fa fa-external-link"></i>**](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)
:::

---

### Emoji
```=
:+1: , :100: , :eyes:
:fire: , :anger: , :ok_hand:
```
> :+1: , :100: , :eyes:
> :fire: , :anger: , :ok_hand:
::: success
想要找更多其他 Emoji 的代號 ，可以看看 [這裡](https://gist.github.com/rxaviers/7360908)
:::
    
---

### 製作表格
```markdow=
| 欄名一 | 欄名二 | 欄名三 |
|:-----:|:-----:|:-----:|
| 元素一 | 元素二 | 元素三 |
| 元素四 | 元素五 | 元素六 |
    
    
|:100: 測試單框格|
|--------------|
```
    
> | 欄名一 | 欄名二 | 欄名三 |
> |:----:|:----:|:----:|
> | 元素一 | 元素二 | 元素三 |
> | 元素四 | 元素五 | 元素六 |
>
>
> |:100: 測試單框格|
> |--------|
    

