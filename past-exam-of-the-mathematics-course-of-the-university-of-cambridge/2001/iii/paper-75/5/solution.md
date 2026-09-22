<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $\mu_N=[PSL_2(\mathbb Z):\overline{\Gamma(N)}]$, where the bar denotes the effective projective image. This is the degree of the [modular curve](../../../../../modular-curve.md) projection, rather than the full $SL_2$ index when $-I$ is not in $\Gamma(N)$.

Reduction modulo $N$ is onto $SL_2(\mathbb Z/N\mathbb Z)$. One proof uses the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) and elementary [matrices](../../../../../matrix.md): over $\mathbb Z/p^r\mathbb Z$, a unimodular first column has a unit entry, so elementary row operations reduce a determinant-one [matrix](../../../../../matrix.md) to the identity. Each elementary [matrix](../../../../../matrix.md) lifts integrally. Over $\mathbb F_p$, the first column has $p^2-1$ choices and the second has $p$ choices with prescribed [determinant](../../../../../determinant.md), giving $p(p^2-1)$. Each subsequent prime-power lift has $p^3$ choices, because the determinant-one linearized condition is one trace equation on four entries. Hence

$$
[SL_2(\mathbb Z):\Gamma(N)]=N^3\prod_{p\mid N}(1-p^{-2}).
$$

For $N=1,2$, the subgroup contains $-I$; for $N\geq3$ it does not. Consequently

$$
\mu_1=1,\qquad\mu_2=6,\qquad
\mu_N=\frac{N^3}{2}\prod_{p\mid N}(1-p^{-2})\quad(N\geq3).
$$

For $N\geq2$ there are no effective elliptic [stabilizer subgroups](../../../../../stabilizer-subgroup.md) in the subgroup. Indeed, write $\gamma=I+NB\in\Gamma(N)$. The [determinant](../../../../../determinant.md) condition gives $\operatorname{tr}\gamma=2-N^2\det B$. A noncentral elliptic element in $SL_2(\mathbb Z)$ has trace $-1,0$ or $1$, none congruent to $2$ modulo $N^2$ for $N\geq2$. Thus the projective action is torsion-free.

All [cusp widths](../../../../../width-of-a-cusp.md) are $N$. At infinity, $T^h$ lies in the effective subgroup exactly when $h$ is divisible by $N$: the alternative $T^h\equiv-I\pmod N$ can only occur for $N=1,2$, and for $N=2$ it imposes the same condition. Every rational [modular cusp](../../../../../cusp-of-a-modular-group.md) is a modular translate of infinity, and the subgroup is normal, so the same width holds there. The sum of [modular cusp](../../../../../cusp-of-a-modular-group.md) [analytic ramification indices](../../../../../ramification-index-of-a-holomorphic-map.md) equals $\mu_N$, giving $\mu_N/N$ [modular cusps](../../../../../cusp-of-a-modular-group.md).

The base $X(1)$ is a sphere. For instance $j=E_4^3/\Delta$ is a [meromorphic function](../../../../../meromorphic-function.md) on it with a single simple pole at the [modular cusp](../../../../../cusp-of-a-modular-group.md) and no other poles, using the nonvanishing of $\Delta$ proved above. It therefore defines a degree-one map to the [Riemann sphere](../../../../../riemann-sphere.md), making the base [genus](../../../../../genus-of-a-surface.md) zero.

The only branch values of $X(N)\to X(1)$ are the two elliptic orbits and the [modular cusp](../../../../../cusp-of-a-modular-group.md). For $N\geq2$, the numbers of points above them and their [analytic ramification indices](../../../../../ramification-index-of-a-holomorphic-map.md) are respectively $\mu_N/2$ with index two, $\mu_N/3$ with index three, and $\mu_N/N$ with index $N$. Applying the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) directly,

$$
\begin{aligned}
2g(X(N))-2
&=-2\mu_N+\frac{\mu_N}{2}(2-1)+\frac{\mu_N}{3}(3-1)+\frac{\mu_N}{N}(N-1)\\
&=\mu_N\left(\frac16-\frac1N\right).
\end{aligned}
$$

This is the [elliptic and cusp ramification for principal level](../../../../../elliptic-and-cusp-ramification-for-principal-level.md) calculation. Level one is the identity projection. The complete result is

$$
\boxed{g(X(1))=g(X(2))=0,\qquad
g(X(N))=1+\frac{N^2(N-6)}{24}\prod_{p\mid N}(1-p^{-2})\quad(N\geq3).}
$$

For example the genera for $N=3,4,5,6,7$ are $0,0,0,1,3$. Keeping the exceptional projective index at level two is essential; applying the factor one-half there would give a nonintegral answer. This agrees with the [principal congruence modular curve genus](../../../../../principal-congruence-modular-curve-genus.md) formula obtained from these branch counts.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
