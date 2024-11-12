
Hochschild 上同调启发自代数拓扑.

[香蕉空间](https://www.bananaspace.org/wiki/Hochschild_%E5%90%8C%E8%B0%83)

## 定义

受代数拓扑中的单纯复形的启发, 我们定义如下概念.

**定义**. **预单纯模** (presimplicial module) 是指一串模 $C_n$ 以及一族态射 $d_i \colon C_n\to C_{n-1}$, 其中 $i=0,\cdots,n$, 且满足 $d_id_j = d_{j-1}d_i\,(0\leq i< j\leq n)$.

> $d_i$ 是一个单纯形的第 $i$ 个面.

预单纯模的态射是与所有 $d_i$ 可交换的一族态射 $f_n\colon C_n \to C'_n$.

预单纯模的态射的同伦是一族态射 $h_i\colon C_n\to C'_{n+1}\,()$

定义 $d=\sum_{i} (-1)^i d_i$, 则 $d^2 = 0$; 由此可定义预单纯模的同调.

设 $k$ 为域, $R$ 为 $k$-代数, $M$ 为 $R$ 双模. 考虑一串模 $C_n(R,M):= M\otimes_k R^{\otimes n}$ 与态射 $d_i\colon M\otimes R^{n} \to M\otimes R^{n-1}$, 定义如下.
$$
d_0\colon (m\otimes r_1\otimes \cdots \otimes r_n) \mapsto (m r_1\otimes r_2\otimes\cdots\otimes r_n),
$$
$$
d_i\colon (m\otimes r_1\otimes \cdots \otimes r_n) \mapsto (m\otimes r_1\otimes\cdots\otimes r_ir_{i+1}\otimes\cdots\otimes r_n),
$$
$$
d_n\colon (m\otimes r_1\otimes \cdots \otimes r_n) \mapsto (r_nm\otimes r_1\otimes\cdots\otimes r_{n-1}).
$$

对于 $M=R$, 记 $C_n(R)=C_n(R,R)$. **Hochschild 同调** $H_\bullet(R,M)$ 即是上述预单纯模的同调; 对于 $M=R$, 记 $HH_n(R) = H_n(R,R)$.

类似地定义 **Hochschild 上同调** $H^\bullet (R,M)$ 为复形 $\operatorname{Hom}(R^{\otimes n},M)$ 的上同调, 其中 $\delta=\sum_i (-1)^i \delta_i$, $\delta_i$ 定义为
$$
(\delta_0 f)(r_1\otimes\cdots\otimes r_n) =r_1 f(r_2\otimes\cdots\otimes r_n),
$$
$$
(\delta_i f) (r_1\otimes \cdots\otimes r_n) = f(r_1\otimes\cdots\otimes r_ir_{i+1}\otimes\cdots\otimes r_n),
$$
$$
(\delta_n f)(r_1\otimes\cdots\otimes r_n) = f(r_1\otimes\cdots \otimes r_{n-1})r_n.
$$
对于 $M=R$, 记 $HH^n(R)=H^n(R,R)$.

## 性质

考虑 $R$ 的中心 $Z(R)$, 可以证明 $H_*(R,M)$ 上有 $Z(R)$-双模结构.

## 与 Tor, Ext 的关系