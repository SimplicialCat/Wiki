
Zariski 景体现了 [[Grothendieck 拓扑]]在代数几何中的作用.

## 定义

设 $k$ 为交换环, Zariski 景可定义在 $k$-代数的范畴上.

> 我们考虑的对象由点集变成了代数. 由于没有 Hilbert 零点定理, 代数簇可能没有足够的 "点", 我们转而考虑其对应的商环 $k[x_1,\cdots,x_n]/I$. 另外, 含幂零元的 $k$-代数可描述 "形变", 例如我们会区分 $x-y=0$ 与 $(x-y)^2=0$.
> 
> 为了在代数范畴上定义 "覆盖", 我们需要模仿 $\mathbb{C}^n$ 上的 Zariski 开集的覆盖. 一个 $k$-代数 $A$ 的覆盖由其一系列元素 $a_1,\cdots,a_n\in A$ 给出, 使得 $1$ 包含在理想 $(a_1,\cdots,a_n)$ 中.

考虑有限表现 (finitely-presented) 的, 即形如 $k[x_1,\cdots,x_n]/(f_1,\cdots,f_m)$ 的 $k$-代数范畴 $k-\mathsf{Alg}_{\text{fp}}$.

一个 $A$ 代数的**覆盖**是一族态射
$$
A\to A[a_i^{-1}]\simeq A[x]/(xa_i - 1),
$$
满足 $1\in (a_1,\cdots,a_n)$.

## 结构层

Zariski 景上有典范的结构[[层]], 它是局部环层.