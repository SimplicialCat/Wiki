
Grothendieck--Riemann--Roch 定理描述了[[陈特征]]沿着[[紧合映射]] (proper map) $f\colon X\to Y$ 的前推与自然性的差距, 其 "矫正项" 与 [[Todd 类]]有关, 仅取决于 $X$ 和 $Y$ 本身.

这个定理可视为 [[Hirzebruch--Riemann--Roch 定理]]的[[相对]]版本.

设 $f\colon X\to Y$ 是光滑代数簇的[[紧合映射]].

令 $K(X)$ 为 $X$ 上的[[凝聚层]]或局部自由层的 Grothendieck 环 (见 [[K-理论]]), 定义同态 $f_k\colon K(X)\to K(Y)$ 为态射 $f$ 的[[导出前推]]的交错和
$$
f_k(F):=\sum (-1)^q R^q f_* F.
$$
[Wiki](https://en.wikipedia.org/wiki/Grothendieck%E2%80%93Riemann%E2%80%93Roch_theorem) 叙述的定理考虑的是 $f_!=\sum (-1)^i R^i f_*\colon K_0(X)\to K_0(Y)$, 其中 $K_0(X)$ 是凝聚层的有界复形的 Grothendieck 群.

考虑[[周环]]的推出映射 $f_*\colon A(X)\to A(Y)$.

**定理** (Grothendieck) 对任意 $\alpha\in K(X)$,
$$
\operatorname{ch}(f_k\alpha) \operatorname{td}(T_Y) = f_*(\operatorname{ch}(\alpha)\operatorname{td}(T_X)).
$$

[[Euler 示性数]] $\chi(X,F)$ 可用[[陈特征]]表示. 当 $Y$ 是一个点时,
$$
\chi(X,F)= \operatorname{ch}\Big(\sum (-1)^q H^q(X,F)\Big).
$$