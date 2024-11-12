Heyting 代数是一个偏序集, 存在所有有限的积和余积, 且构成[[Descartes 闭范畴|积闭范畴]]. 换言之, Heyting 代数中有 $0$, $1$, 指数对象 $y^x$ (通常记作 $x\Rightarrow y$), 而指数对象由如下的伴随关系刻画:
$$
z\leq (x\Rightarrow y) \quad \text{iff} \quad z\wedge x \leq y.
$$

## 性质

由基本伴随关系, 可得 (实际上是伴随的单位和余单位态射)
$$
x\leq \big( y\Rightarrow (x\wedge y) \big),\quad y\wedge (y\Rightarrow x) \leq x.
$$
而由 $1^x\simeq 1$, $x^1\simeq x$ 可得
$$
(x\Rightarrow 1) =1,\quad (1\Rightarrow x) =x.
$$
由于函子 $x\Rightarrow -$ 有右伴随, 它保持极限, 即
$$
(x\Rightarrow (y\wedge z)) = \big( (x\Rightarrow y) \wedge (x \Rightarrow z)\big).
$$
等式 $x^{y\times z}\simeq (x^y)^z$ 成为
$$
((y\wedge z)\Rightarrow x) = (z\Rightarrow (y\Rightarrow x)).
$$

## 例

对拓扑空间 $X$, 其上开集构成的偏序集为 Heyting 代数. 对于开集 $U, V$,
$$
(U \Rightarrow V) = \bigcup_{W\cap U\subset V} W.
$$
每个 [[Boole 代数]]都是 Heyting 代数, 反之则不然.