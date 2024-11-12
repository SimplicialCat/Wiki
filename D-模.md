
D-模简而言之就是微分算子环上的模.

## 起源: 微分方程组

经典的微分方程理论研究的是方程组
$$
\sum_{j=1}^p R_{ij} u_j =0,\quad 1\leq i \leq q,
$$
其中 $R_{ij}$ 为线性微分算子, $u_j$ 为变量 $x_1,\cdots,x_n$ 的函数.

以代数的语言叙述这个问题, 设 $A$ 是某个函数环, 如光滑函数环, 复解析函数环, 多项式环等等. 设 $\mathcal{D}$ 是 $A$-系数的微分算子的环. 微分算子 $R_{i,j}$ 构成了左 $\mathcal D$-模的态射
$$
R\colon \mathcal D^p \to \mathcal D^q.
$$
现在设微分方程的解所生活的空间是另一个 $\mathcal D$-模 $N$ (例如 $A$ 本身). 微分方程的解可表示为态射 $u\colon \mathcal D^q\to N$, 而微分方程组则可表示为复合 $u\circ R = 0$.

定义 $\mathcal D$-模 $M=\operatorname{coker}R$, 由余核的泛性质, 微分方程的解等同于 $\operatorname{Hom}_{\mathcal D}(M,N)$.
$$
\begin{array}{ccccccccc}
0 & \to & \mathcal D^p & \overset{R}{\to} & \mathcal D^q &\to & M & \to & 0\\
&&&&& \hspace{-1em}u\searrow & \downarrow &&\\
&&&&&& N &&
\end{array}
$$
这就是说, **微分方程组等同于有限表现的左 $\mathcal D$-模**.

我们需要处理微分方程局部的解; 而一个解沿闭合路径一周的解析延拓可能与原来不同, 这种现象称作**单值** (monodromy). 因此我们需要研究局部的解如何连接起来成为整体的解. 这时[[层]]论是处理这种问题最合适的语言. 将环 $A$ 与模 $\mathcal D$ "变为层", 就得到 $X$ 上的微分算子层 $D_X$.

我们研究的主要对象是**局部有限表现**的 $D_X$-模, 也即[[凝聚层|凝聚]] $D_X$-模. 我们最关心的函子是
$$
\mathcal Hom_{D_X}(-,\mathcal O_X)\colon \mathsf {Mod}_{\text{coh}}(D_X) \to \mathsf {Mod}(\mathbb{C}_X),
$$
而它不是正合函子; 故我们需考虑它的[[导出函子]]即 "高阶解" $\mathcal Ext^\bullet_{D_X}(-,\mathcal O_X)$.

### 特征簇

设 $p=q=1$, $R$ 的[[特征簇]]是

## 定义

设 $X$ 是 $\mathbb C$ 上的光滑代数簇. $X$ 上的 D-模是[[正则微分算子]]层 $D_X$ 上的模. 左 $D_X$-模即带有 $D_X$ 作用的 $\mathcal{O}_X$-模, 等同于线性映射
$$
\nabla\colon D_X \to \operatorname{End}_{\mathbb C}(M),
$$
满足

- $\nabla_{fv}(m)=f\nabla_v(m)$;
- $\nabla_v(fm)=v(f) m + f\nabla_v m$;
- $\nabla_{[v,w]}m=[\nabla_v,\nabla_w]m$.

$X$ 上的 D-模也可视为带有[[可积联络|平坦联络]]的拟凝聚 $\mathcal{O}_X$-模.

## 函子性

与凝聚层类似, 不同代数簇上的 D-模由推出和拉回联系起来.

## 和乐

设 $M$ 为凝聚 $D_X$-模. 若其[[特征簇]]满足 $\dim \operatorname{Ch}(M)=\dim X$, 即特征簇的维数取到**最小**可能值, 则称 $M$ 为**和乐** (holonomic) 的.

和乐 $D_X$-模是线性常微分方程在高维复流形的自然推广.

## 微局部

D-模可定义为 [[de Rham 空间]]上的拟凝聚层.

## 例

### 向量丛

设 $E$ 是 $X$ 上带有[[可积联络|平坦联络]] $\nabla$ 的向量丛, 也即局部形如 $\bigoplus_i \mathcal O_U e_i$ 的层.

回忆联络 $\nabla$ 可视为丛映射 $TX\to \operatorname{End}(E)$, 满足

- $\nabla_{av}=a\nabla_v$;
- $\nabla_v(as)=v(a)s+a\nabla_v s$;
- $\nabla_{[v,w]}=[\nabla_v,\nabla_w]$ (称为可积性或平坦性; 见[[可积联络]]).

此时左 $D_X$-模结构即由 $v\cdot s = \nabla_v s$ 给出.

### 对偶层

对偶层 $\omega = \det \Omega^1$

由于 Lie 导数 $L_v = [\iota_v, d]$, 对于 $\alpha\in\omega$ 有 $L_v\alpha = d \iota_v \alpha$.

对偶层可以把右 D-模变成左 D-模:
$$
D^{\text{op}} = \omega\otimes D \otimes \omega^{-1}
$$

### 摩天大楼 D-模

$p\in X$, 定义
$$
M_p = D_X / D_X ()
$$