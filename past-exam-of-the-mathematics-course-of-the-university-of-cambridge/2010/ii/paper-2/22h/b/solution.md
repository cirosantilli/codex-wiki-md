<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $x^{(n)}\in c_0$ converges uniformly to $x$. Choose $n$ with $\|x-x^{(n)}\|_\infty<\varepsilon/2$, then a tail on which $|x_j^{(n)}|<\varepsilon/2$. On this tail $|x_j|<\varepsilon$, proving $x\in c_0$. Linearity is coordinatewise, so **$c_0$ is a closed subspace.**

For $a\in\ell^1$, define the [bounded linear functional](../../../../../../continuous-linear-functional.md) $L_a(x)=\sum_ja_jx_j$. Absolute convergence gives $\|L_a\|\leq\|a\|_1$. For each $m$, take $x_j=\overline{a_j}/|a_j|$ when $1\leq j\leq m$ and $a_j\ne0$, and zero elsewhere. This finitely supported sequence belongs to $c_0$ and has norm at most one, giving $\|L_a\|\geq\sum_{j=1}^m|a_j|$. Therefore $\|L_a\|=\|a\|_1$.

Conversely, for $L\in c_0^*$ put $a_j=L(e_j)$. The same finite phase vectors give $\sum_{j=1}^m|a_j|\leq\|L\|$, so $a\in\ell^1$. The finite truncations of every $x\in c_0$ converge in the [supremum norm](../../../../../../supremum-norm.md), hence continuity gives $L(x)=\lim_m\sum_{j=1}^ma_jx_j=L_a(x)$. This proves the surjective [isometric isomorphism of normed spaces](../../../../../../isometric-isomorphism-of-normed-spaces.md) **$\boxed{c_0^*\cong\ell^1}$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
