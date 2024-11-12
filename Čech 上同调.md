
## 定义

设 $X$ 为拓扑空间, $\mathcal F$ 为其上的预[[层]].

设 $\mathscr U =(U_\alpha)$ 为 $X$ 的 (局部有限) 开覆盖. 下面我们定义 $\mathscr U$ 上取值在 $\mathcal F$ 中的上链复形
$$
0\to C^0(\mathscr U,\mathcal F)\to C^1(\mathscr U,\mathcal F) \to \cdots.
$$

上链群 $C^k(\mathscr U,\mathcal F)$ 的元素是如下的函数 $\varphi$: 对于每个 $(k+1)$-元组 (也叫 $k$-**单形**, simplex) $(\alpha_0,\cdots,\alpha_k)$ 都指定一个截面 $\varphi(\alpha_0,\cdots,\alpha_k)\in \Gamma (U_{\alpha_0}\cap\cdots\cap U_{\alpha_k} , \mathcal F)$.

上边缘 $\delta$ 的定义为
$$
\delta\varphi(\alpha_0,\cdots,\alpha_{k+1})=\sum_i (-1)^i \varphi(\alpha_0,\cdots,\widehat{\alpha_i},\cdots,\alpha_{k+1}).
$$
(我们默认对于右边的求和项施加适当的限制映射.)

复形 $C^\bullet(\mathscr U,\mathcal F)$ 的上同调即为 Čech 上同调 $\check H^\bullet(\mathscr U,\mathcal F)$.

设开覆盖 $\mathscr V = (V_j)_{j\in J}$ 是 $\mathscr U = (U_i)_{i\in I}$ 的**加细** (refinement), 也即存在映射 $\lambda \colon J\to I$, 使得对任意 $j\in J$, $V_j$ 包含于 $U_{\lambda (j)}$. 定义链映射
$$
\lambda_{\mathscr V}^{\mathscr U} \colon  C^k(\mathscr U,\mathcal F) \to C^k(\mathscr V, \mathcal F),
$$
$$
(\lambda_{\mathscr V}^{\mathscr U} \varphi)(j_0,\cdots,j_k) := \varphi(\lambda (j_0),\cdots,\lambda (j_k)),
$$
可验证 $\lambda_{\mathscr V}^{\mathscr U}$ 与上边缘 $\delta$ 交换, 于是有上同调之间的同态 $\check H^\bullet (\mathscr U,\mathcal F) \to \check H^\bullet(\mathscr V,\mathcal F)$. 进一步, 可证明上同调的同态与映射 $\lambda \colon  J\to I$ 的选取无关 (不同的映射 $\lambda$ 得到的链映射 $\lambda_{\mathscr V}^{\mathscr U}$ 相差一个 "棱镜" 链同伦).

我们可对所有开覆盖取顺向极限, 得到 $X$ 上系数在 $\Gamma$ 中的 Čech 上同调:
$$
\check H^\bullet(X,\mathcal F)=\lim_{\longrightarrow} \check H^\bullet(\mathscr{V},\mathcal F).
$$

## 性质

### 函子性

设 $\mathcal S,\mathcal T$ 为 Abel 群 (或一般的模) 层, $h\colon  \mathcal S \to \mathcal T$ 是同态, 则对任意局部有限开覆盖 $\mathscr U$ 有链映射 $h\colon  C^\bullet(\mathscr U,\mathcal S) \to C^\bullet (\mathscr U,\mathcal T)$, 从而有同态 $h\colon \check H^\bullet (\mathscr U,\mathcal S) \to \check H^\bullet (\mathscr U,\mathcal T)$, $h\colon \check H^\bullet (X,\mathcal S) \to \check H^\bullet (X,\mathcal T)$.

### 正合列

**命题**. 层的短正合列
$$
0\to \mathcal F' \to \mathcal F \to \mathcal F'' \to 0,
$$
诱导 Čech 上同调的长正合列
$$
0 \to H^0(X,\mathcal F')\to H^0(X,\mathcal F) \to H^0(X,\mathcal F'')
\overset{\delta}{\to} H^1(X,\mathcal F') \to \cdots.
$$

细节. 映射 $C^p(\mathscr U,\mathcal F) \to C^p(\mathscr U,\mathcal F'')$ 不一定是满射, 但可以选取更细的开覆盖 $\mathscr W$, 使得对任意 $c''\in C^p(\mathscr W,\mathcal F'')$ 存在 $c\in C^p(\mathscr U,\mathcal F)$ 限制到 $c''$.

连接同态 $\delta$ 的定义. 对 $[c'']\in H^p(\mathscr U,\mathcal F'')$, 取 $[c]\in C^p(\mathscr U,\mathcal F)$, 那么 $\delta c\in C^{p+1}(X,\mathcal F)$ 来自 $c'\in C^{p+1}(X,\mathcal F')$. 定义 $\delta[c'']=[c']$.

### 与层上同调的关系

设 $\mathcal F$ 为 $X$ 上的预层, 则总有 Čech 上同调到其层化 $\mathcal F^+$ 的[[层上同调]]的映射
$$
\check H^n(X,\mathcal F) \to H^n(X,\mathcal F^+),
$$
但不一定是同构. 当 $X$ 是仿紧 Hausdorff 空间时, 上述映射是同构.

## 例

### 0 维上同调

$H^0(\mathscr U, \mathcal F)$ 的元素是上圈 $(\varphi_i)$, 满足任意两个截面 $\varphi_i$ 与 $\varphi_j$ 在相交处 $U_{ij}$ 都相等; 这就是说 $H^0(\mathscr U, \mathcal F)$ 的元素是 $\mathcal F$ 的[[整体截面]] (这个事实与开覆盖 $\mathscr U$ 的选取无关).

### 主丛

设有 $X$ 上的 $G$-主丛 $E\to X$, $\mathscr{U}=(U_\alpha)$ 是平凡化覆盖,
$\varphi_\alpha\colon U_\alpha\times G\to E$ 是局部坐标.
转移函数 $\varphi_{\alpha\beta}\colon U_\alpha\cap U_\beta\to G$ 满足
$$
\varphi_{\alpha\gamma}=\varphi_{\alpha\beta}\circ \varphi_{\beta\gamma}.
$$
换言之, 对于 $1$-上链 $\varphi\colon (\alpha,\beta)\mapsto \varphi_{\alpha\beta}$, 有
$$
\delta\varphi(\alpha,\beta,\gamma)=\varphi_{\beta\gamma}\circ\varphi_{\alpha\gamma}^{-1}\circ\varphi_{\alpha\beta} =1.
$$
(这里为了确切符合上面定义的形式, 还需要 $G$ 为 Abel 群.)
因此这个条件称为**上圈条件** (cocycle condition). 见[[非 Abel 上同调]].

### Mittag-Leffler 问题

设 $X$ 为复流形, $O$ 为 $X$ 上的全纯函数层, 则 [[Mittag-Leffler 问题]]
(?)

### 代数几何

一般地, 对具有拓扑的[[景]], 如 [[Zariski 景]], 概形的[[平展景]], 都可定义 Čech 上同调.
