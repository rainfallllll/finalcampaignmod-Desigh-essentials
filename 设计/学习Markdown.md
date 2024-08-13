
|难度  | 范围  |
|:---:|:---:| 
|低度&中度|1|
|高度&极高|2|
|毁灭|3|


       - 低度 和 中度---半径1 威胁度1
      - 高度 和 极高---半径1 威胁度2          半径2 威胁度1
      - 毁灭---半径1 威胁度4          半径2 威胁度2        半径3 威胁度1
      根据威胁度计算该区块难度
      低度-------1
      中度-------2
      高度-------3
      极高-------5
      毁灭-------6
  


| 威胁度  | 半径1  | 半径2  | 半径3  |  
|:---:|:---:|:---:|:---:|
|低度&中度|1|none|none|
|高度&极高|2|1|none|
|毁灭|4|2|1|  


| 难度  | 威胁度 |     |     |
| :-: | :-: | --- | --- |
| 低度  |  1  |     |     |
| 中度  |  2  |     |     |
| 高度  |  3  |     |     |
| 极高  |  5  |     |     |
| 毁灭  |  6  |     |     |



- [ ] 这个软件用的咧

- 一、公式形式
- 二、公式多行表达式
    - 1, 多行表达式
    - 2, 方程组
    - 3, 分类表达式
    - 4, 注释方程式
- 三、公式中字母
- 四、公式中的常见符号
    - 1, 上下标
    - 2, 括号与分割符
    - 3, 分式和根式
- 五、公式中的运算符
    - 1, 关系运算符
    - 2, 集合运算符
    - 3, 对数运算符
    - 4, 三角运算符
    - 5, 微积分运算符
    - 6, 逻辑运算符
- 六、公式中的其他符号
    - 1, 戴帽符号
    - 2, 连线符号
    - 3, 箭头符号
    - 4, 其他符号
- 七、公式中表格与矩阵
    - 1, 表格
    - 2, 矩阵

### **一、公式形式**

markdown中公式使用

LaTex

数学公式, 一般分为两种形式：内联公式和公式块，即行内公式和行间公式：

内联公式：

Φ(t)=∫∞0zt−1e−zdz.

公式块：

Φ(t)=∫∞0zt−1e−zdz.

javascript

```javascript
$\Phi(t) = \int_0^\infty z^{t-1}e^{-z}dz\,.$
$$\Phi(t) = \int_0^\infty z^{t-1}e^{-z}dz\,.$$
```

### **二、公式多行表达式**

#### **1, 多行表达式**

a=(b+c)×d+(e−f)=g+h=i

javascript

```javascript
$$
\begin{equation}\begin{split} 
a&=(b+c)\times{d} \\ 
&\quad +(e-f)\\ 
&=g+h\\ 
& =i 
\end{split}\end{equation}
$$
```

> 公式中`\begin{equation}...\end{equation}` 表示方程开始与结束；`\begin{split}...end{split}` 表示开始多行公式开始与结束；`\\` 表示回车到下一行，`&` 表示对齐的位置

#### **2, 方程组**

⎧⎪⎨⎪⎩a1x+b1y+c1z=d1a2x+b2y+c2z=d2a3x+b3y+c3z=d3

javascript

```javascript
$$
\left \{ 
\begin{array}{c}
a_1x+b_1y+c_1z=d_1 \\ 
a_2x+b_2y+c_2z=d_2 \\ 
a_3x+b_3y+c_3z=d_3
\end{array}
\right.
$$
```

> 公式中`\left \{ ... \right.`表示方程的左边和右边，`\begin{array}...\end{array}` 表示方程组的开始与结束，再配合表示方程组得到公式。 `.`表示空格, 但`a..b`与`a.b`都会显示`ab`。如需要显示`a b`，可用`\`增加些许空隙, `\;`与`\quad{}`增加较宽间隙, `\qqaud{}`增加更大间隙。

#### **3, 分类表达式**

- 表达式一

f(n)⎧⎨⎩n2,if n is even3n2+n+1,if n is odd

javascript

```javascript
$$
f(n)
\begin{cases}
\cfrac n2, &if\ n\ is\ even\\
3n^2 + n+1, &if\  n\ is\ odd
\end{cases}
$$
```

- 表达式二

L(Y,f(X))=⎧⎪⎨⎪⎩0,Y = f(X)1,Y ≠ f(X)

javascript

```javascript
$$
L(Y,f(X)) =
\begin{cases}
0, & \text{Y = f(X)} \\[4ex]
1, & \text{Y $\neq$ f(X)}
\end{cases}
$$
```

> 可以使用`\\[4ex]` 代替`\\` 来将分类之间的垂直间隔变大。其中`[4ex]` 中的数字代表间隔距离，`1ex` 相当于原始距离，数字越大，距离越大。

#### **4, 注释方程式**

在 `{align}` 中灵活组合 `\text` 和 `\tag` 语句。`\tag` 语句编号优先级高于自动编号。

javascript

```javascript
$$
\begin{align}
   v + w & = 0  &\text{Given} \tag 1\\
   -w & = -w + 0 & \text{additive identity} \tag 2\\
   -w + 0 & = -w + (v + w) & \text{equations $(1)$ and $(2)$} \tag 3
\end{align}
$$
```

v+w=0Given−w=−w+0additive identity−w+0=−w+(v+w)equations (1) and (2)(1)(2)(3)

### **三、公式中字母**

|name|大写|code|小写|code|
|---|---|---|---|---|
|alpha|A|A|α|\alpha|
|beta|B|B|β|\beta|
|gamma|Γ|\Gamma|γ|\gamma|
|delta|Δ|\Delta|δ|\delta|
|epsilon|E|E|ϵ|\epsilon|
|zeta|Z|Z|ζ|\zeta|
|eta|H|H|η|\eta|
|theta|Θ|\Theta|θ|\theta|
|iota|I|I|ι|\iota|
|kappa|K|K|κ|\kappa|
|lambda|Λ|\Lambda|λ|\lambda|
|mu|M|M|μ|\mu|
|nu|N|N|ν|\nu|
|xi|Ξ|\Xi|ξ|\xi|
|omicron|O|O|ο|\omicron|
|pi|Π|\Pi|π|\pi|
|rho|P|P|ρ|\rho|
|sigma|Σ|\Sigma|σ|\sigma|
|tau|T|T|τ|\tau|
|upsilon|υυ|υ|υ|\upsilon|
|phi|Φ|\Phi|ϕ|\phi|
|chi|X|X|χ|\chi|
|psi|Ψ|\Psi|ψ|\psi|
|omega|Ω|\Omega|ω|\omega|
|ell_p|||ℓp|\ell_p|

> 变量专用形式`\var-`

|code|小写|code|大写|var-code|变量|
|---|---|---|---|---|---|
|\epsilon|ϵ|E|E|\varepsilon|ε|
|\theta|θ|\Theta|Θ|\vartheta|ϑ|
|\rho|ρ|P|P|\varrho|ϱ|
|\sigma|σ|\Sigma|Σ|\varsigma|ς|
|\phi|ϕ|\Phi|Φ|\varphi|φ|

### **四、公式中的常见符号**

#### **1, 上下标**

- 上标和下标分别使用^ 与_ ，例如x2i
- 默认情况下，上、下标符号仅仅对下一个组起作用。一个组即单个字符或者使用`{..}` 包裹起来的内容。
- 上下标可以嵌套，也可以同时使用。xyz=(1+ex)−2xyw
- 如果要在左右两边都有上下标，可以用 \sideset 命令。12⨂34

#### **2, 括号与分割符**

|code|显示|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|---|---|
|\langle|⟨|\rangle|⟩|\lceil|⌈|\rceil|⌉|
|\lfloor|⌊|\rfloor|⌋|\lbrace|{|\rbrace|}|

- 使用原始的`( )` , `[ ]`, `|` 即表示符号本身。
- 使用`\left(`或`\right)`使符号大小与邻近的公式相适应, 该语句适用于所有括号类型, 即显示大括号或分割符。
- 使用 `\left.` 或 `\right.` 进行匹配而不显示本身。
- `\lceil` 和 `\rceil` 表示上取整；`\lfloor` 和 `\rfloor`表示下取整

例1: f(x,y,z)=8y2z(8+8x+21+y2) 显示为:

f(x,y,z)=8y2z(8+8x+21+y2)

例2: 积分:dydx∣∣x=0 显示为:

dydx∣∣∣x=0

例3: 偏导: ∂2y∂x2 显示为:

∂2y∂x2

#### **3, 分式和根式**

- **分式**
    - `\frac {分子} {分母}`
- 命令产生一个分数，分数可嵌套。a+c+1b+c+2 显示为:便捷情况可直接输入 \frac ab 来快速生成:
    - 使用\over来分隔一个组的前后两部分，在分数很复杂时使用，如a+1b+1 显示为:
- 连分数

`\frac`或者`\over` 的使用

javascript

```javascript
$$
x=a_0 + \frac {1^2}{a_1 + \frac {2^2}{a_2 + \frac {3^2}{a_3 + \frac {4^2}{a_4 + ...}}}}
$$
```

x=a0+12a1+22a2+32a3+42a4+...

`\cfrac`的使用

javascript

```javascript
$$
x=a_0 + \cfrac {1^2}{a_1 + \cfrac {2^2}{a_2 + \cfrac {3^2}{a_3 + \cfrac {4^2}{a_4 + ...}}}}
$$
```

javascript

x=a0+12a1+22a2+32a3+42a4+...

x=a0+12a1+22a2+32a3+42a4+...

- **根式**
    - `\sqrt [根指数，省略时为2] {被开方数}`
    - 开3次方：3√xy 显示为:
    - 开平方：√a+b 显示为:

### **五、公式中的运算符**

#### **1, 关系运算符**

|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|
|\pm|±|\times|×|\div|÷|
|\nmid|∤|\mid|∣|\cdot|⋅|
|\ldots|…|\cdots|⋯|\circ|∘|
|\bigodot|⨀|\bigotimes|⨂|\bigoplus|⨁|
|\geq|≥|\neq|≠|\approx|≈|
|\leq|≤|\lt|<|\gt|>|
|\sum|∑|\prod|∏|\coprod|∐|
|\approx|≈|\sim|∼|\equiv|≡|
|\star|⋆|\ast|∗|\bullet|∙|
|\prec|≺|\succ|≻|\oplus|⊕|
|\preceq|⪯|\succeq|⪰|\pmod n|(mod n)|

求和

- ∑nr=1 显示为:

连乘

- ∏a+b 显示为:

K∏i=1

显示为:

省略号

javascript

```javascript
$$
a_1+a_2+\ldots+a_n 
a_1+a_2+\cdots+a_n 
$$
```

显示为：

a1+a2+…+ana1+a2+⋯+an

javascript

```javascript
$$
f(x_1,x_2,\underbrace{\ldots}_{\rm ldots} ,x_n) = x_1^2 + x_2^2 + \underbrace{\cdots}_{\rm cdots} + x_n^2
$$
```

显示为：

f(x1,x2,…ldots,xn)=x21+x22+⋯cdots+x2n

- `\ldots` 表示与文本底线对齐的省略号, 位置稍低

其他

argmaxck ​显示为

argmaxck

- argminck 显示为:
- argmaxck 显示为:
- minck 显示为:

可以在运算符前面加`\not`，如`\not\lt` :

≮

`\ldots` 位置稍低，`\cdots` 位置居中

#### **2, 集合运算符**

|code|name|显示|code|显示|code|显示|
|---|---|---|---|---|---|---|
|\emptyset|空集|∅|\in|∈|\notin|∉|
|\subset|子集|⊂|\supset|⊃|\supseteq|⊇|
|\subseteq|子集|⊆|\bigcap|⋂|\bigcup|⋃|
|\setminus|差集|∖|\cap|∩|\cup|∪|
|\varnothing|空|∅|\bigvee|⋁|\bigwedge|⋀|
|\subsetneq|非空集|⊊|\biguplus|⨄|||

#### **3, 对数运算符**

|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|
|\log|log|\lg|lg|\ln|ln|

#### **4, 三角运算符**

|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|
|30^\circ|30∘|\bot|⊥|\angle A|∠A|
|\sin|sin|\cos|cos|\tan|tan|
|\csc|csc|\sec|sec|\cot|cot|
|\arcsin|arcsin|\arccos|arccos|\arctan|arctan|

#### **5, 微积分运算符**

|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|
|\int|∫|\iint|∬|\iiint|∭|
|\iiiint|⨌|\oint|∮|\prime|′|
|\lim|lim|\infty|∞|\nabla|∇|

积分

- `\int_积分下限^积分上限 {被积表达式}` 来输入一个积分。
- ∫10x2dx,其中 \, 和 {\rm d} 部分可省略，建议加入，使式子更美观。显示：

极限

javascript

```javascript
$$
\lim_{n \to +\infty} \frac{1}{n(n+1)} \quad or \quad \lim_{x\leftarrow{sample}} \frac{1}{n^2+1} 
$$
```

显示为：

limn→+∞1n(n+1)orlimx←sample1n2+1

- `\lim_{变量 \to 表达式} 表达式`

#### **6, 逻辑运算符**

| code     | 显示  | code       | 显示  | code        | 显示  |
| -------- | --- | ---------- | --- | ----------- | --- |
| \because | ∵   | \therefore | ∴   |             |     |
| \forall  | ∀   | \exists    | ∃   | \not\subset | ⊄   |
| \not<    | $   | \not>      | ≯   | \not=       | ≠   |
| \land    | ∧   | \lnot      | ¬   | \exists     | ∃   |
| \lor     | ∨   | \forall    | ∀   | \top        | ⊤   |
| \bot     | ⊥   | \vdash     | ⊢   | \vDash      | ⊨   |

### **六、公式中的其他符号**

#### **1, 戴帽符号**

![](https://ask.qcloudimg.com/http-save/yehe-8756457/7uf9azzbaa.jpeg)

- 矢量→a⋅→b=0 显示为:
    - `\vec{矢量}`自动产生一个矢量

→a⋅→b=0

- `\overrightarrow` 等命令自定义字母上方的符号。

javascript

```javascript
$$
\overleftarrow{xy} \quad or \quad \overleftrightarrow{xy} \quad or \quad \overrightarrow{xy}
$$
```

显示为：

←−xyor←→xyor−→xy

#### **2, 连线符号**

![](https://ask.qcloudimg.com/http-save/yehe-8756457/otymf27zaj.jpeg)

### **七、公式中表格与矩**

#### **3, 箭头符号**

|code|显示|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|---|---|
|\rightarrow|→|\leftarrow|←|\longrightarrow|⟶|\longleftarrow|⟵|
|\Rightarrow|⇒|\Leftarrow|⇐|\Longrightarrow|⟹|\Longleftarrow|⟸|
|\uparrow|↑|\downarrow|↓|\mapsto|↦|\to|→|
|\Uparrow|⇑|\Downarrow|⇓|\Longleftrightarrow|⟺|||

#### **4, 其他符号**

|name|code|显示|code|显示|code|显示|
|---|---|---|---|---|---|---|
|排列|\binom{n+1}{2k}||{n+1 \choose 2k}||||
|范围|\infty|∞|\aleph_o|ℵo|\nabla|∇|
|范围|\Im|ℑ|\Re|ℜ|||

### **七、公式中表格与矩阵**

#### **1, 表格**

nLeftCenterRight12511252−11+10i−1310014

javascript

```javascript
$$
\begin{array}{c|lcr}
n & \text{Left} & \text{Center} & \text{Right} \\
\hline
1 & 25 & 1 & 125 \\
2 & -1 & 1+10i & -1 \\
3 & 100 & 1 & 4 \\
\end{array}
$$
```

> `\begin{array}{列样式}…\end{array}` 形式来创建表格，列样式可以是`clr` 表示居中，左，右对齐，还可以使用`|` 表示一条竖线。表格中各行使用`\\` 分隔，各列使用`&` 分隔。使用`\hline` 在本行前加入一条直线

#### **2, 矩阵**

1xx2x31yy2y31zz2z3

javascript

```javascript
$$
\begin{matrix}
1 & x & x^2 & x^3 \\
1 & y & y^2 & y^3\\
1 & z & z^2 & z^3\\
\end{matrix}
$$
```

- **矩阵的括号** `\left{matrix}...\right{matrix}` , 其中`matrix` 可替换为为`pmatrix`，`bmatrix`，`Bmatrix`，`vmatrix` , `Vmatrix`

- (1234)
- [1234]
- ∣∣∣1234∣∣∣
- ∥∥∥1234∥∥∥
- **矩阵中元素省略** `\cdots` :

⋯

，`\ddots`:

⋱

，`\vdots`：

⋮

来省略矩阵中的元素

javascript

```javascript
$$
\begin{pmatrix}
1&a_1&a_{12}&\cdots&a_{1n}\\
1&a_2&a_{22}&\cdots&a_{2n}\\
\vdots&\vdots&\vdots&\ddots&\vdots\\
1&a_m&a_{m2}&\cdots&a_{mn}\\
\end{pmatrix}
$$
```

⎛⎜ ⎜ ⎜ ⎜ ⎜⎝1a1a12⋯a1n1a2a22⋯a2n⋮⋮⋮⋱⋮1amam2⋯amn⎞⎟ ⎟ ⎟ ⎟ ⎟⎠

- 增广矩阵 `\begin{array} ... \end{array}`

javascript

```javascript
$$
\left[  \begin{array}  {c c | c} %这里的c表示数组中元素对其方式：c居中、r右对齐、l左对齐，竖线表示2、3列间插入竖线
1 & 2 & 3 \\
\hline %插入横线，如果去掉\hline就是增广矩阵
4 & 5 & 6
\end{array}  \right]
$$
```

[123456]

- 交换图标

javascript

```javascript
$$
\begin{CD}
    A @>>> B @>{\text{very long label}}>> C \\
    @. @AAA @| \\
    D @= E @<<< F
\end{CD}
$$
```

A−−−−→Blabel−−−−→C↑⏐⏐∥∥D=====E←−−−−F

> `@>>>` 代表右箭头、`@<<<` 代表左箭头、`@VVV` 代表下箭头、`@AAA` 代表上箭头、`@=` 代表水平双实线、`@|` 代表竖直双实线、`@.`代表没有箭头,在 `@>>>` 的 `>>>` 之间任意插入文字即代表该箭头的注释文字