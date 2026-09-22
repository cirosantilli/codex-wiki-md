<h1 id="11h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\chi(x)=(x/p)$. Choose a [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) $a$. Multiplication by $a$ permutes $\mathbb F_p$, while [multiplicativity of the Legendre symbol](../../../../../../multiplicativity-of-the-legendre-symbol.md) gives $\chi(ax)=-\chi(x)$. Therefore

$$
\sum_{x\in\mathbb F_p}\chi(x)
=\sum_{x\in\mathbb F_p}\chi(ax)
=-\sum_{x\in\mathbb F_p}\chi(x),
$$

so the [complete Legendre-symbol sum](../../../../../../complete-legendre-symbol-sum.md) is zero.

Since $4x(x+1)=(2x+1)^2-1$ and $\chi(4)=1$, the bijection $x\mapsto2x+1$ reduces the next sum to $\sum_y\chi(y^2-1)$. Count pairs $(y,t)\in\mathbb F_p^2$ satisfying $t^2=y^2-1$. On one hand their number is

$$
\sum_y\bigl(1+\chi(y^2-1)\bigr).
$$

On the other hand $(y-t)(y+t)=1$, and every $u\in\mathbb F_p^\times$ gives exactly one pair by $y-t=u$, $y+t=u^{-1}$. There are therefore $p-1$ pairs, proving the [quadratic Legendre-symbol correlation](../../../../../../quadratic-legendre-symbol-correlation.md)

$$
\sum_{x\in\mathbb F_p}\chi(x(x+1))=-1.
$$

For $1\leq z\leq p-2$, the indicator that both $z$ and $z+1$ are quadratic residues is $(1+\chi(z))(1+\chi(z+1))/4$. Summing and using the two identities above gives the [number of consecutive nonzero quadratic residues modulo an odd prime](../../../../../../number-of-consecutive-nonzero-quadratic-residues-modulo-an-odd-prime.md)

$$
\frac14\left(p-2-\chi(-1)-1-1\right)
=\boxed{\frac{p-4-(-1)^{(p-1)/2}}4}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11H](../../11h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
