<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiply the growth equation by $2\eta^2(1+\eta)$:

$$
2\eta^2(1+\eta)D_{\eta\eta}+\eta(3+4\eta)D_\eta-3D=0.
$$

Use the [Frobenius method](../../../../../../frobenius-method.md), writing $D=\sum_{n\geq0}b_n\eta^{\alpha+n}$ with $b_0\ne0$. The lowest power gives the [indicial equation](../../../../../../indicial-equation.md)

$$
2\alpha(\alpha-1)+3\alpha-3=(\alpha-1)(2\alpha+3)=0.
$$

Thus the leading powers are $\alpha=1$ and $\alpha=-3/2$. For $n\geq1$, equating the coefficient of $\eta^{\alpha+n}$ gives

$$
(\alpha+n-1)[2(\alpha+n)+3]b_n
+2(\alpha+n-1)(\alpha+n)b_{n-1}=0.
$$

For the growing branch $\alpha=1$, $b_n=-2(n+1)b_{n-1}/(2n+5)$, so $b_1=-4b_0/7$ and $b_2=8b_0/21$. Taking $b_0=A_k$,

$$
\boxed{\delta_C=A_k\eta\left[1-\frac47\eta+\frac8{21}\eta^2+O(\eta^3)\right].}
$$

Since $\eta\propto a$, the leading behavior is precisely the usual growing [density contrast](../../../../../../density-contrast.md) $\delta_C\propto a\propto t^{2/3}$ during [matter domination](../../../../../../matter-domination.md). The negative first correction shows the beginning of suppressed growth as the string fraction increases. The other branch starts as $a^{-3/2}$, the familiar decaying matter mode; its exact form is proportional to $\sqrt{1+\eta}/\eta^{3/2}$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
