<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume piecewise-constant real controls with freely chosen duration, as in the usual finite-dimensional [quantum controllability](../../../../../../quantum-controllability.md) theorem. We can establish the strongest notion here: **the [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md) is $\mathfrak u(3)$, so the system has [unitary operator controllability](../../../../../../unitary-operator-controllability.md)**, and consequently both pure-state and fixed-spectrum [density operator controllability](../../../../../../density-operator-controllability.md).

To verify the hypotheses explicitly, use [matrix units](../../../../../../matrix-unit.md) $E_{jk}=|j\rangle\langle k|$ and put $K_0=-iH_0$, $X_{jk}=-i(E_{jk}+E_{kj})$, $Y_{jk}=E_{jk}-E_{kj}$. Then $K_1=-iH_1=d_1X_{12}+d_2X_{23}$ and

$$
\operatorname{ad}_{K_0}^2K_1=-\omega_1^2d_1X_{12}-\omega_2^2d_2X_{23}.
$$

Since $d_1d_2\ne0$ and $\omega_1^2\ne\omega_2^2$, linear combinations of these two elements isolate $X_{12}$ and $X_{23}$. Their [commutators](../../../../../../commutator.md) with $K_0$ give $\omega_1Y_{12}$ and $-\omega_2Y_{23}$, respectively. Further [commutators](../../../../../../commutator.md) give two independent traceless diagonal generators, since $[X_{jk},Y_{jk}]=2i(E_{jj}-E_{kk})$, as well as the two $1$–$3$ generators. These eight generators span the [special unitary Lie algebra](../../../../../../special-unitary-lie-algebra.md) $\mathfrak{su}(3)$.

Finally $\operatorname{Tr}K_0=i(\omega_1+\omega_2)\ne0$. Subtract its traceless component, already in the generated algebra, to obtain a nonzero multiple of $iI$. This proves the [Lie algebra of the unitary group](../../../../../../unitary-lie-algebra.md) is all of $\mathfrak u(3)$, not merely $\mathfrak{su}(3)$. The compact-group [controllability](../../../../../../controllability.md) theorem then gives access to every unitary with a suitable control and some duration. This does not assert [controllability](../../../../../../controllability.md) at every predetermined short time or under additional bandwidth constraints. This proves that [two adjacent transitions generate the qutrit unitary Lie algebra](../../../../../../two-adjacent-transitions-generate-the-qutrit-unitary-lie-algebra.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
