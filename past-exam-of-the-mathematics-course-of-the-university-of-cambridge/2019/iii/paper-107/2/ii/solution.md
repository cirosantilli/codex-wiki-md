<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) here states

$$
Lu\geq0\text{ in }\Omega\quad\Longrightarrow\quad
\max_{\overline\Omega}u\leq\max_{\partial\Omega}u
$$

for $u\in C^2(\Omega)\cap C^0(\overline\Omega)$.

To prove it, suppose the interior maximum exceeds the boundary maximum. Put $q(x)=e^{-\ell x_1}$. Since $c=0$,

$$
Lq=q(\ell^2a^{11}-\ell b^1)
\geq q\ell(\lambda\ell-|b^1|)>0.
$$

For sufficiently small $\varepsilon>0$, $u_\varepsilon=u+\varepsilon q$ still has an interior maximum. At that point its [gradient](../../../../../../gradient.md) vanishes and its [Hessian matrix](../../../../../../hessian-matrix.md) is negative semidefinite; ellipticity gives $Lu_\varepsilon\leq0$. But $Lu_\varepsilon=Lu+\varepsilon Lq>0$, a contradiction. This proves the principle.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
