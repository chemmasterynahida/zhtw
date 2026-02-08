---
title: "量子化學：1.1. 黑體輻射"
published: 2025-10-05
description: "黑體輻射理論遇到了什麼問題？又是如何被解決的？"
image: "https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/planck.png"
tags: ["量子化學"]
category: 量子化學
lang: zh_CN
draft: false
---

# 黑體輻射

## 量子化學：導論

你好呀～這是化學精通納西妲。  
今天，我們要開啟第一節關於「量子化學」的課程——一個連光與能量都遵循奇妙微觀法則的世界。  

在開始之前，我們需要先了解「量子」這個詞的含義。  
你可能早就聽説過它，對吧？是不是覺得它聽起來有點未來感？比如「量子計算機」，就是現在非常熱門的技術呢！  
![quantum computer](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/qc.jpg "Quantum Computer by Google")

不過，「量子」到底是什麼意思呢？  
如果你想到「quantity（量）」這個詞，那就非常接近了！「quantum」正是由它演變而來，意思是「某種事物的最小單位」。  
當你了解量子力學誕生的故事時，這個詞就會變得清晰明了。  

## 普朗克之前（1900年之前）

讓我們回到十九世紀末，去看看一個讓物理學家百思不得其解的問題——**黑體輻射**。  
**牛頓**早在他的著作《光學》中就提到過類似的現象：  

> "Do not black Bodies conceive heat more easily from Light than those of other Colours do, by reason that the Light falling on them is not reflected outwards, but enters the Bodies, and is often reflected and refracted within them, until it be stifled and lost?"  
>
> “黑色物體不是比其他顏色的物體更容易從光中産生熱量嗎？因爲照射在黑色物體上的光不會向外反射，而是進入物體內部，並經常在物體內部反射和折射，直到被抑製和消失？”  

黑色的物體會吸收所有可見光，而不反射任何光。  
那麼，光的能量被吸收後會怎樣呢？能量應該守恆的。  
1858年，**Balfour Stewart** 發現黑體既能最強地吸收能量，也能最強地發射能量。  
一年後，**Gustav Kirchhoff** 進一步指出，黑體輻射的光譜只與溫度有關，與材料本身無關。  
隨後，科學家們提出了許多公式來描述這種神秘的發光現象。  
其中，**Wien（維恩）** 在1896年的公式與實驗非常吻合：  

**維恩定律 (1896)**  
$$u(\nu,T)=a\nu^{3}e^{-b\nu/T}$$  
$u$: 單位體積、單位頻率下的能量密度  
$\nu$: 頻率  
$T$: 溫度  
$a, b$: 常數  

1900年6月，**Rayleigh（瑞利）** 基於經典理論提出了另一個公式：  
**瑞利–金斯定律 (1900)**  
$$du(\nu,T)=\frac{8\pi\nu^{2}}{c^{3}}Ud\nu=\frac{8\pi\nu^{2}kT}{c^{3}}d\nu$$  
$c$: 光速 ($c=299792458~m/s$)  
$k$: 玻爾茲曼常數 ($k=1.380649×10^{−23}~J/K$)  

然而……事情出了問題。  
在高頻區域，這個公式竟然預示能量會無窮大！  
物理學家稱之爲 **「紫外災難」**。  
![ultraviolet catastrophe](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/planck.png "\"Ultraviolet catastrophe\"")  
瑞利–金斯定律在低頻率準確，而維恩定律在高頻率成立。  
但兩者之間，卻存在著一道無法跨越的鴻溝。  

---
## 量子物理的誕生

1900年12月，**馬克斯·普朗克（Max Planck）** 靈光一閃：  
“如果光的能量不是連續的……而是由一個個微小能量包組成的呢？”  

他稱這些最小能量單位爲 **「量子（quantum）」**。  

**量子假設**  
$$E=n\epsilon=nh\nu$$  
$\epsilon$: 光的最小能量單元  
$h=6.62607015\times10^{-34}~J\cdot s$: 普朗克常數  
$\nu$: 頻率  

這便是**量子物理的種子**。  
「量子」這個詞，從此代表——**能量的最小單位**。  

## 普朗克定律

爲了描述這些量子能量如何分佈，普朗克引入了 **玻爾茲曼分布**：  

**玻爾茲曼分布**  
$$f(E)\propto e^{\frac{E}{kT}}$$  
$f(E)$: 擁有能量 $E$ 的粒子數  
$k$: 玻爾茲曼常數  
$T$: 溫度  

通過推導，可以得到平均能量。這方法不是來自普朗克，是玻色與愛因斯坦的想法(1924)。  
$$<E>=<f(n\epsilon)>=\frac{\sum_{n=0}^{\infty}n\epsilon e^{-n\epsilon/kT}}{\sum_{n=0}^{\infty}e^{-n\epsilon/kT}}=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{h\nu}{e^{h\nu/kT}-1}$$  
將其與常數結合，我們得到：  
**普朗克輻射定律（按頻率表示）**  
$$du(\nu,T)=\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  

**普朗克輻射定律（按波長表示）**  
$$du(\lambda,T)=\frac{8\pi hc}{\lambda^{5}}\cdot\frac{1}{e^{hc/\lambda kT}-1}d\lambda$$  

終於，一條方程連接了維恩定律與瑞利–金斯定律——理論與實驗的和諧交響曲。

## 普朗克定律的驗證

一條優秀的理論，必須經得起實驗的考驗。  
普朗克的方程完美解釋了兩條已知的經驗定律：  

**斯特藩–玻爾茲曼定律 (1877)**  
*輻射功率與溫度的四次方成正比*：  
$$M=\sigma T^{4}$$  

**維恩位移定律 (1896)**  
*輻射峰值波長與溫度成反比*：  
$$\lambda_{peak}=\frac{b}{T}$$  

兩者都可從普朗克定律中推導而來。  

### 斯特藩–玻爾茲曼定律的推導

對所有頻率積分，可得總輻射能量：  
我們也可以從中獲取地表輻射。  

> $$\int du=\int_{0}^{\infty}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  
> 令 $x=h\nu/kT$，因此 $dx=hd\nu/kT$，可以進行變量替換：  
> $$\int_{0}^{\infty}\frac{8\pi k^{3}T^{3}}{h^{2}c^{3}}\cdot\frac{x^{3}}{e^{x}-1}\cdot\frac{kT}{h}dx$$  
> 這個積分的值是已知的：  
> $$\int_{0}^{\infty}\frac{x^{3}}{e^{x}-1}dx=\frac{\pi^{4}}{15}$$  
> 因此,  
> $$E=\int du=\frac{8\pi k^{3}T^{3}}{h^{2}c^{3}}\cdot\frac{\pi^{4}}{15}\cdot\frac{kT}{h}=\frac{8\pi^{5}k^{4}T^{4}}{15h^{3}c^{3}}$$  
> 這樣，我們就得到了黑體輻射的總輻射能量（單位：$J/m^{3}$）。不過，斯特藩–玻爾茲曼定律討論的是輻射功率（單位：$W/m^{2}$）。我們可以通過乘上 $c/4$，將體積能量轉換爲單位面積的輻射功率：
> $$M=E\cdot\frac{c}{4}=\frac{8\pi^{5}k^{4}T^{4}}{15h^{3}c^{3}}\cdot\frac{c}{4}=\frac{2\pi^{5}k^{4}T^{4}}{15h^{3}c^{2}}=\sigma T^{4}$$  

**斯特藩–玻爾茲曼定律**  
$$M=\sigma T^{4}=\frac{2\pi^{5}k^{4}}{15h^{3}c^{2}}T^{4}$$  
$$\sigma=\frac{2\pi^{5}k^{4}}{15h^{3}c^{2}}=5.67\times10^{-8}W/m^{2}\cdot K^{4}$$  
這個數值與實驗結果完全吻合～  

### 維恩位移定律的推導

維恩位移定律（Wien’s displacement law） 描述的是在什麼波長（或頻率）下，黑體的輻射最強。  
輻射強度的峰值波長爲：  

> $$\frac{d(du/d\lambda)}{d\lambda}=0$$  
> 普朗克定律也可以用波長來表示：  
> $$\frac{du(\lambda,T)}{d\lambda}=\frac{8\pi hc}{\lambda^{5}}\cdot\frac{1}{e^{hc/\lambda kT}-1}$$  
> 爲了簡化方程，我們令 $\lambda=hc/xkT$，於是有 $d\lambda=-hcdx/x^{2}kT$。  
> $$du(x,T)=-\frac{8\pi x^{5}k^{5}T^{5}}{h^{4}c^{4}}\cdot\frac{1}{e^{x}-1}dx$$  
> 接下來，我們要找出使得下式成立的 $x$：  
> $$\frac{d}{dx}(\frac{x^{5}}{e^{x}-1})=\frac{5x^{4}(e^{x}-1)-x^{5}(e^{x})}{(e^{x}-1)^{2}}=0$$  
> 通過數值計算可以得到：  
> $$x=\frac{hc}{\lambda kT}\approx4.9651$$  
> 因此，這個關係可以寫作：  
> $$\lambda_{peak}=\frac{b}{T}\approx\frac{hc}{4.9651kT}=\frac{2.90mm/K}{T}$$  

**維恩位移定律**  
$$\lambda_{peak}=\frac{b}{T}\approx\frac{hc}{4.9651kT}=\frac{2.90mm/K}{T}$$  
溫度越高，輻射峰值越短——  
所以，熾熱的物體會從紅光逐漸變爲黃光、再到藍白光。  

### $\nu\rightarrow0$

瑞利–金斯定律（Rayleigh–Jeans law） 能很好地解釋低頻情況下的實驗結果。在低頻極限下（$\nu$ 很小時），普朗克定律應當趨近於瑞利–金斯定律：  

> $$\lim_{\nu\rightarrow0}du(\nu,T)=\lim_{\nu\rightarrow0}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  
> 已知極限：  
> $$\lim_{x\rightarrow0}\frac{e^{x}-1}{x}=1$$  
> 因此方程可化爲：  
> $$\lim_{\nu\rightarrow0}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu=\frac{8\pi kT\nu^{2}}{c^{3}}d\nu$$  

當頻率很小時，普朗克定律就會收斂爲瑞利–金斯定律。  

### $\nu\rightarrow\infty$

而在高頻極限下，維恩定律（Wien’s law） 則更符合實驗結果。對於較大的頻率 $\nu$，普朗克定律會收斂爲維恩定律：  

> $$\lim_{\nu\rightarrow\infty}du(\nu,T)=\lim_{\nu\rightarrow\infty}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu$$  
> 由於指數函數增長極快，我們可以近似認爲 $e^{h\nu/kT}-1 \approx e^{h\nu/kT}$。
> $$\lim_{\nu\rightarrow\infty}\frac{8\pi h\nu^{3}}{c^{3}}\cdot\frac{1}{e^{h\nu/kT}-1}d\nu=\frac{8\pi h\nu^{3}}{c^{3}}\cdot e^{-h\nu/kT}d\nu=a\nu^{3}e^{-b\nu/T}$$  

因此，在高頻時，普朗克定律的形式會非常接近維恩定律。  

---
---

## 普朗克的思考與啟發

### 1900年10月：連接兩種理論

普朗克注意到，維恩定律與瑞利–金斯定律各自只在特定範圍內成立。  
他思考著——是否存在一種更深層的聯係，使兩者成爲同一個真理的不同面貌呢？  

經過對熱力學與熵的研究，他推導出了一條能夠平滑連接二者的新方程。  

> 對於 維恩定律（Wien’s law） 而言，能量與頻率和溫度的關係是一個指數函數；而在 瑞利–金斯定律（Rayleigh–Jeans law） 中，能量則與溫度成正比。  
> $$U_{Wien}\propto \nu e^{-b\nu/T}~(Wien)$$  
> $$U_{RJ}\propto T~(RJ)$$  
> 普朗克首先從熱力學的角度來研究這個問題。熱力學第一定律可以寫作：  
> $$dU=TdS-PdV$$  
> 在黑體輻射實驗中，實驗裝置是一個帶有微小孔洞的封閉腔體，因此系統體積幾乎不變。  
> ![experiment](https://gcore.jsdelivr.net/gh/chemmasterynahida/assets/common/blackbody-radiation/experiment.jpg "Blackbody Radiation Experiment")  
> 因此可以簡化爲：  
> $$dU=TdS,~\frac{\partial S}{\partial U}=\frac{1}{T}$$  
> 普朗克分別考慮了兩條定律下熵隨能量的變化關係：  
> $$\frac{\partial S}{\partial U}=\frac{1}{T}\propto ln(U)~(Wien)$$  
> $$\frac{\partial S}{\partial U}=\frac{1}{T}\propto\frac{1}{U}~(RJ)$$  
> 那麼，我們再對它求一次導數看看會發生什麼呢？  
> $$\frac{\partial^{2} S}{\partial U^{2}}\propto\frac{1}{U}~(Wien)$$  
> $$\frac{\partial^{2} S}{\partial U^{2}}\propto\frac{1}{U^{2}}~(RJ)$$  
> 因此，可以把 $(\partial^{2} S/\partial U^{2})^{-1}$ 看作能量 $U$ 的多項式形式：  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}\propto U~(Wien''s)$$  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}\propto U^{2}~(RJ)$$  
> 普朗克將兩種形式結合起來：  
> $$(\frac{\partial^{2} S}{\partial U^{2}})^{-1}=C_{1}U+C_{2}U^{2}$$  
> 最終，他得出了這樣對波長的方程形式：  
> $$U=\frac{C\lambda^{-5}}{e^{c/\lambda T}-1}$$  

### 1900年12月：能量的離散化

隨後，普朗克藉助玻爾茲曼的統計原理，假設腔體中的能量由無數「能量元」組成。  
$$\epsilon\epsilon\epsilon|\epsilon\epsilon|\epsilon|\epsilon\epsilon\epsilon|\epsilon\epsilon|\cdots$$  
$\epsilon$：能量元  

他用組合數學計算這些能量元的排列數：  
$$W=\frac{(P+N-1)!}{P!(N-1)!}$$  
$P=UN/\epsilon$: 能量粒子數量, $U$:一個光波的能量  
$N$: 光波數量  

> 因爲 $N$ 的數值非常大，我們可以將 $N-1$ 近似爲 $N$。
> 同時，當數值 $n$ 足夠大時，階乘可用斯特林公式近似表示爲：  
> $$n!\approx\sqrt{2\pi n}(n/e)^{n}~(n\rightarrow\infty)$$  
> 由於 $n^{n}$ 相比 $\sqrt{n}$ 要大得多，因此可以寫成：  
> $$W=\frac{(P+N-1)!}{P!(N-1)!}\approx \frac{(P+N)^{P+N}}{P^{P}N^{N}}$$  

並通過玻爾茲曼關係式與熵聯係起來。  
$$S=k\cdot ln(W)$$  
$S$: 系的絶對熵量  
$W$: "*Wahrscheinlichkeit*", 微觀狀態數量  

> 讓我們回憶一下熱力學中的公式：  
> $$\frac{1}{T}=\frac{\partial S}{\partial U}=k\frac{\partial(ln(W))}{\partial U}$$  
> 我們已經得到了 $W$ 的近似形式，因此可以寫出：  
> $$ln(W)=(P+N)ln(P+N)-Pln(P)-Nln(N)=\frac{N}{\epsilon}((U+\epsilon)ln(U+\epsilon)-\epsilon ln(\epsilon)-Uln(U))$$  
> 因此，  
> $$\frac{kN}{\epsilon}(ln(U+\epsilon)-ln(U))$$  
> 對於單個能量單元而言，其熵爲：  
> $$\frac{k}{\epsilon}(ln(U+\epsilon)-ln(U))=\frac{1}{T}$$  
> 於是我們就得到了：  
> $$U=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{hv}{e^{hv/kT}-1}$$  

最終，他得到了那個改變物理史的結果：  
$$U=\frac{\epsilon}{e^{\epsilon/kT}-1}=\frac{hv}{e^{hv/kT}-1}$$  

這正是普朗克那條著名的方程。  
光的能量，只能以 $h\nu$ 的整數倍存在。  
它揭示了能量不是連續的，而是由一個個離散的量子組成的。  
他因發現能量子而榮獲1918年諾貝爾物理學獎。  

> *1918年諾貝爾物理學獎授予馬克斯·卡爾·恩斯特·路德維希·普朗克，"因他的對量子的發現而推動物理學的發展"。*  

從此，人類的目光第一次觸及了量子世界的門檻——那一刻，知識的光，悄悄地在科學的夜空中亮起。  
這標誌了量子時代的黎明。  
人類第一次窺見了宇宙最微小的秘密。  

## 參考文獻

Blackbody Radiation: Wikipedia (<https://en.wikipedia.org/wiki/Blackbody%20Radiation>)  
Planck''s Law: Wikipedia (<https://en.wikipedia.org/wiki/Planck%27s%20Law>)  
Planck, M. (1900). Über eine Verbesserung der Wien’schen Strahlungsgleichung. *Verhandlungen der Deutschen Physikalischen Gesellschaft*.  
Planck, M. (1900). Zur theorie des gesetzes der energieverteilung im normalspektrum. *VhDPG*, 2, 238.  
