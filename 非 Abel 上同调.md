
## 1 阶非 Abel 上同调

设 $\mathcal G$ 是拓扑空间 $X$ 上的群层.

对 $X$ 的开覆盖 $\mathcal U=\{U_\alpha\}$, 一个 $1$-**上圈** (cocycle) 是一族截面 $g_{\alpha\beta}\in \mathcal G(U_{\alpha\beta})$, 在 $U_{\alpha\beta\gamma}$ 上满足
$$
g_{\alpha\beta} g_{\beta\gamma} = g_{\alpha\gamma}.
$$
两个 $1$-上圈**等价**是指存在一族 $f_\alpha\in\mathcal G(U_\alpha)$ 满足
$$
f_\alpha g_{\alpha\beta} = h_{\alpha\beta} f_\beta.
$$
$1$-上圈的等价类记为 $H^1(\mathcal U,\mathcal G)$, 而其余极限记为
$$
\check H^1(X,\mathcal G):=\lim_{\longrightarrow} H^1(\mathcal U,\mathcal G).
$$
**定理**. $X$ 上 $G$-[[主丛]]的同构类一一对应于 $\check H^1(X,\mathcal G)$ 的元素.

