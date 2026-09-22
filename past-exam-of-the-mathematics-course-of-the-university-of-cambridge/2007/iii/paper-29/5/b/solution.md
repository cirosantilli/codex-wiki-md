<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reduction modulo $N$ has [kernel](../../../../../../kernel-of-a-linear-map.md) $\Gamma(N)$ and is onto $SL_2(\mathbb Z/N\mathbb Z)$. To see [surjectivity](../../../../../../surjective-function.md), use the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) to reduce to $\mathbb Z/p^a\mathbb Z$. In that local ring a unimodular column has a unit entry. Elementary row operations move a unit to the upper position and clear the lower one; diagonal [matrices](../../../../../../matrix.md) $\operatorname{diag}(u,u^{-1})$ are products of elementary [matrices](../../../../../../matrix.md) as well. Explicitly, with $E_{12},E_{21}$ denoting elementary shears,

$$
\begin{pmatrix}0&u\\-u^{-1}&0\end{pmatrix}
=E_{12}(u)E_{21}(-u^{-1})E_{12}(u),
$$

and multiplying this by the same [matrix](../../../../../../matrix.md) with $u=-1$ gives $\operatorname{diag}(u,u^{-1})$. Thus elementary [matrices](../../../../../../matrix.md) generate the special linear group over each local ring. Chinese remaindering their parameters gives generation over the product ring, and every such parameter lifts to an integer. This proves the reduction is onto.

Over $\mathbb F_p$, there are $p^2-1$ choices for a nonzero first column and $p$ choices for a second column with [determinant](../../../../../../determinant.md) one, so $|SL_2(\mathbb F_p)|=p(p^2-1)$. Each reduction from modulus $p^{a+1}$ to $p^a$ has [kernel](../../../../../../kernel-of-a-linear-map.md) represented by $I+p^aB$, with $B$ modulo $p$ and $\operatorname{tr}B=0$, of size $p^3$. Hence, for $N>1$,

$$
[SL_2(\mathbb Z):\Gamma(N)]
=|SL_2(\mathbb Z/N\mathbb Z)|
=N^3\prod_{p\mid N}(1-p^{-2}).
$$

For $N=1$ the index is one. Since $-I\in\Gamma(N)$ exactly when $N=1,2$,

$$
\mu=\begin{cases}1&N=1,\\6&N=2,\\
\frac{N^3}{2}\displaystyle\prod_{p\mid N}(1-p^{-2})&N\geq3.
\end{cases}
$$

For $N\geq2$ there are no nontrivial effective elliptic stabilizers. Indeed $A=I+NB\in\Gamma(N)$ with [determinant](../../../../../../determinant.md) one has $\operatorname{tr}B=-N\det B$, and therefore

$$
\operatorname{tr}A=2-N^2\det B\equiv2\pmod{N^2}.
$$

A noncentral elliptic element of $SL_2(\mathbb Z)$ has [trace](../../../../../../matrix-trace.md) $0$ or $\pm1$, none congruent to $2$ modulo $N^2$ for $N\geq2$. The central element $-I$ at level two acts trivially and is not an [elliptic point](../../../../../../elliptic-point.md) of the effective quotient. Thus $\nu_2=\nu_3=0$ for $N\geq2$, while at level one both numbers are one.

The subgroup $\Gamma(N)$ is normal, so all its [modular cusps](../../../../../../cusp-of-a-modular-group.md) have the same effective width as infinity. That width is $N$: the shear $T^h$ belongs to $\pm\Gamma(N)$ exactly when $N\mid h$; for $N\geq3$ its diagonal entries exclude the minus sign, and for $N=1,2$ that sign changes nothing. Since [modular cusp](../../../../../../cusp-of-a-modular-group.md) widths sum to $\mu$,

$$
\nu_\infty=\frac{\mu}{N}
=\begin{cases}1&N=1,\\3&N=2,\\
\frac{N^2}{2}\displaystyle\prod_{p\mid N}(1-p^{-2})&N\geq3.
\end{cases}
$$

For $N\geq3$ the resulting [principal congruence modular curve genus](../../../../../../principal-congruence-modular-curve-genus.md) is

$$
\boxed{g(X(N))=1+\frac{N^2(N-6)}{24}\prod_{p\mid N}(1-p^{-2}).}
$$

For clarity, the small levels, including all exceptional terms, are

$$
\begin{array}{c|rrrrrr}
N &[SL_2:\Gamma(N)]&\mu&\nu_2&\nu_3&\nu_\infty&g\\\hline
1&1&1&1&1&1&0\\
2&6&6&0&0&3&0\\
3&24&12&0&0&4&0\\
4&48&24&0&0&6&0\\
5&120&60&0&0&12&0\\
6&144&72&0&0&12&1
\end{array}
$$

For $N>6$, every factor in the [genus](../../../../../../genus-of-a-surface.md) correction is positive, so $g>1$. Therefore **the genus-zero levels are exactly $N=1,2,3,4,5$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
