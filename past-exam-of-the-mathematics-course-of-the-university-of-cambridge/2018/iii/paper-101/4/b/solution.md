<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes: $R[[x]]$ is Noetherian.** We prove [Noetherianity of a formal power series ring](../../../../../../noetherianity-of-a-formal-power-series-ring.md) directly, using only the equivalence in part (a). Let $A=R[[x]]$, a [formal power series ring](../../../../../../formal-power-series.md), and fix an [ideal](../../../../../../ideal.md) $I\subseteq A$. For $n\geq0$, let $C_n$ be the set of coefficients of $x^n$ in elements of $I\cap x^nA$. It is an [ideal](../../../../../../ideal.md) of $R$, because coefficient extraction is additive and respects multiplication by constants. Multiplication by $x$ gives

$$
C_0\subseteq C_1\subseteq C_2\subseteq\cdots.
$$

Since $R$ is [Noetherian](../../../../../../noetherian-ring.md), there is an $N$ with $C_n=C_N$ for all $n\geq N$. Each $C_n$, for $0\leq n\leq N$, has a finite [generating set of an ideal](../../../../../../generating-set-of-an-ideal.md) $a_{n1},\ldots,a_{nr_n}$. Choose $f_{nj}\in I\cap x^nA$ whose coefficient of $x^n$ is $a_{nj}$. If $C_n=0$, use no generators at that index.

We claim that these finitely many $f_{nj}$ generate $I$ over $A$. Given $f\in I$, start with $g_0=f$ and recursively construct $g_n\in I\cap x^nA$. For $n<N$, express the coefficient of $x^n$ in $g_n$ as $\sum_jc_{nj}a_{nj}$, with $c_{nj}\in R$, and subtract $\sum_jc_{nj}f_{nj}$ to obtain $g_{n+1}\in I\cap x^{n+1}A$. For $n\geq N$, use $C_n=C_N$ and subtract

$$
\sum_jc_{nj}x^{n-N}f_{Nj}
$$

to cancel that coefficient. Every step involves a finite sum and leaves a residual still in $I$.

For each $j$, define the [formal power series](../../../../../../formal-power-series.md)

$$
h_j(x)=\sum_{n=N}^{\infty}c_{nj}x^{n-N}\in A.
$$

The residual after the $n$th cancellation lies in $x^{n+1}A$, so comparison of each coefficient gives the exact identity

$$
f=\sum_{n=0}^{N-1}\sum_jc_{nj}f_{nj}+\sum_jh_j(x)f_{Nj}.
$$

The right side is a finite $A$-linear combination of the chosen generators. No assertion that arbitrary [ideals](../../../../../../ideal.md) are closed under limits is being used: the equality is verified coefficient by coefficient, and the multipliers $h_j$ belong to $A$. Thus every [ideal](../../../../../../ideal.md) of $A$ is finitely generated, proving

$$
\boxed{R\text{ Noetherian}\ \Longrightarrow\ R[[x]]\text{ Noetherian}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
