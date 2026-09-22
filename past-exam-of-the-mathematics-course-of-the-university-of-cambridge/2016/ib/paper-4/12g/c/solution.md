<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First $w\in\ell^2$, since $\sum_{n\geq1}4^{-n}=1/3$. Any finite [linear dependence](../../../../../../linear-dependence.md) among $w$ and the $e_m$ has the form $aw+\sum_{m\in F}b_me_m=0$ for a finite index set $F$. At an index outside $F$, its coordinate equals $a2^{-n}$, so $a=0$. Each remaining coordinate then gives $b_m=0$. Therefore the set is [linearly independent](../../../../../../linear-independence.md), and the prescribed values define a unique [linear map](../../../../../../linear-map.md) on its algebraic [span](../../../../../../linear-span.md).

Take the tails

$$
v_N=w-\sum_{m=1}^N2^{-m}e_m.
$$

They belong to $V$, satisfy $f(v_N)=1$, and have

$$
\boxed{\|v_N\|_2^2=\sum_{n>N}4^{-n}=\frac{4^{-N}}3\longrightarrow0.}
$$

Thus $v_N\to0$ while $f(v_N)$ does not approach $f(0)=0$. **The map is not continuous**, and part (b) also shows it is unbounded. This is a [discontinuous functional detected by vanishing sequence tails](../../../../../../discontinuous-functional-detected-by-vanishing-sequence-tails.md), illustrating why the finite-dimensional conclusion in part (a) cannot be extended to arbitrary normed spaces.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
