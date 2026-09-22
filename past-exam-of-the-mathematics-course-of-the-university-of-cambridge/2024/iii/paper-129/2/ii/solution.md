<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $B=\mathbb F_2^n\setminus(A+A)$ have density $\beta$. Since $1_A*1_A$ vanishes on $B$,

$$
0=\langle1_A*1_A,1_B\rangle
=\sum_t\widehat{1_A}(t)^2\widehat{1_B}(t).
$$

The zero-frequency contribution is $\alpha^2\beta$, so

$$
\alpha^2\beta
\le\sum_{t\ne0}|\widehat{1_A}(t)|^2|\widehat{1_B}(t)|.
$$

Put $\Gamma=\operatorname{Spec}_{\alpha/2}(1_B)$. Outside $\Gamma$, [Parseval identity](../../../../../../parseval-identity.md) bounds the contribution by

$$
\frac{\alpha\beta}{2}\sum_t|\widehat{1_A}(t)|^2
=\frac{\alpha^2\beta}{2}.
$$

Therefore

$$
\sum_{t\in\Gamma\setminus\{0\}}|\widehat{1_A}(t)|^2\ge\frac{\alpha^2}{2},
$$

because $|\widehat{1_B}(t)|\le\beta$. Chang's theorem places $\Gamma$ in a subspace $W$ of dimension

$$
O(\alpha^{-2}\log(\beta^{-1})).
$$

Set $V=W^\perp$. Then $V$ has this codimension, $V^\perp=W$, and adding the zero-frequency term $|\widehat{1_A}(0)|^2=\alpha^2$ gives

$$
\boxed{\sum_{t\in V^\perp}|\widehat{1_A}(t)|^2\ge\frac{3\alpha^2}{2}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
