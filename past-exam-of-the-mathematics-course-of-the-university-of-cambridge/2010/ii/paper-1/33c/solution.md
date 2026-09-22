<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

The unique maximum-$M$ product state is

$$
\boxed{|J,J\rangle=|j_1,j_1\rangle_1|j_2,j_2\rangle_2,
\quad J=j_1+j_2.}
$$

Apply the total lowering operator $J_-=J_{1-}+J_{2-}$ and normalize to obtain that multiplet. At the next highest remaining $M$, choose a normalized vector orthogonal to all previously constructed multiplets and annihilated by $J_+$. It is the next highest-weight state; lower it in the same way. Iterating produces every allowed total [angular momentum](../../../../../angular-momentum.md) and the [Clebsch-Gordan coefficients](../../../../../clebsch-gordan-coefficients.md).

For equal constituent spins, a total-spin singlet has $M=0$, so only the product basis vectors with opposite magnetic quantum numbers can occur. Acting with $J_+$ on the expansion and examining the coefficient of $|j,m+1\rangle_1|j,-m\rangle_2$ gives

$$
(\alpha_m+\alpha_{m+1})\sqrt{(j-m)(j+m+1)}=0,
\qquad -j\leq m<j.
$$

Thus $\alpha_{m+1}=-\alpha_m$. Normalization requires $(2j+1)|\alpha_m|^2=1$. Choosing a conventional overall phase gives

$$
\boxed{|0,0\rangle=\frac1{\sqrt{2j+1}}
\sum_{m=-j}^j(-1)^{j-m}|j,m\rangle_1|j,-m\rangle_2.}
$$

The exponent is an integer even for half-integral $j$. Projecting the specified extreme product state onto this unique singlet gives the measurement probability

$$
\boxed{\mathbb P(J=0)=\frac1{2j+1}.}
$$

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
