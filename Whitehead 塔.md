
## 陈述

对任意连通空间 $X$, 存在一列[[纤维化]] $\cdots\to P_2\to P_1$, 以及相容的映射 $X\to P_i$,
$$
\begin{array}
	{ccccc}
	&&\vdots\\
	&&\downarrow\\
	&&W_3&\leftarrow & K(\pi_3(X),3)\\
	&\swarrow&\downarrow\\
	&&W_2&\leftarrow & K(\pi_2(X),2)\\
	&\swarrow&\downarrow\\
	X & \leftarrow & W_1
\end{array}
$$
满足

- $W_n$ 的不超过 $n$ 阶同伦群平凡, 即 $W_n$ $n$-连通;
- 映射 $W_n\to X$ 在超过 $n$ 阶同伦群上为同构;
- 对于 $n\geq 2$, 映射 $W_n\to W_{n-1}$ 的纤维为 [[Eilenberg--MacLane 空间]] $K(\pi_n(X),n-1)$.

> nLab: The Whitehead tower of a pointed homotopy type $X$ is an interpolation of the point inclusion $* \to X$ by a sequence of homotopy types $*\to\cdots\to W_2\to W_1\to X$ that are obtained from right to left by removing homotopy groups from below.

nLab 指出 $W_n$ 是同伦纤维
$$
\begin{array}
	{ccc}
	W_n & \to & *\\
	\downarrow && \downarrow\\
	X & \to & P_{n+1}.
\end{array}
$$
## 例

$$
\cdots\to \text{String}(n)\to\text{Spin}(n)\to SO(n) \,(\to O(n))
$$
## 相关概念

[[Postnikov 塔]]