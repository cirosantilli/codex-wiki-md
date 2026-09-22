<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $p=2+4/d$. For $u_{a,\lambda}(x)=au(\lambda x)$, the [change of variables](../../../../../../change-of-variables-formula.md) $y=\lambda x$ gives

$$
\|\nabla u_{a,\lambda}\|_2^2
=|a|^2\lambda^{2-d}\|\nabla u\|_2^2,\qquad
\|u_{a,\lambda}\|_2^{4/d}
=|a|^{4/d}\lambda^{-2}\|u\|_2^{4/d},
$$

and

$$
\|u_{a,\lambda}\|_p^p
=|a|^{2+4/d}\lambda^{-d}\|u\|_p^p.
$$

The factors cancel, so the [Weinstein functional](../../../../../../weinstein-functional.md) satisfies $J(u_{a,\lambda})=J(u)$.

The [Gagliardo-Nirenberg interpolation inequality](../../../../../../gagliardo-nirenberg-interpolation-inequality.md) gives

$$
\|u\|_p^p\leq C_d\|\nabla u\|_2^2\|u\|_2^{4/d}.
$$

**Consequently $J(u)\geq C_d^{-1}$ for every nonzero $u\in H^1$, and therefore $I>0$.**

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
