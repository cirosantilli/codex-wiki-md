<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [globally coupled underdominant metapopulation](../../../../../../globally-coupled-underdominant-metapopulation.md) with equal habitat sizes:

$$
\dot u_i=f(u_i)+\sigma(\bar u-u_i),
\qquad f(u)=su(1-u)(2u-1),\qquad
\bar u=\frac1N\sum_i u_i.
$$

Symmetry preserves a common frequency $x$ in the initially $AA$ habitats and $y$ in the initially $aa$ habitats. With $q=m/N$, the equations reduce exactly to

$$
\dot x=f(x)-\sigma(1-q)(x-y),\qquad
\dot y=f(y)+\sigma q(x-y),\qquad (x(0),y(0))=(1,0).
$$

The maximum positive selection rate is $f(u_m)=s/(6\sqrt3)$ at $u_m=(3+\sqrt3)/6$. Comparing it with the worst outward migration flux gives a sufficient barrier condition $\sigma\max(q,1-q)<f(u_m)/u_m$. A slightly stronger optimized condition follows from maximizing the per-capita restoring term $f(u)/u=s(1-u)(2u-1)$ over $u>1/2$: its maximum is $s/8$ at $u=3/4$.

Indeed, on $x=3/4$, with $0\le y\le1/4$, $\dot x\ge3s/32-(3/4)\sigma(1-q)>0$. On $y=1/4$, with $3/4\le x\le1$, $\dot y\le-3s/32+(3/4)\sigma q<0$. The other two edges point inward as well. The [invariant-rectangle criterion for underdominant coexistence](../../../../../../invariant-rectangle-criterion-for-underdominant-coexistence.md) therefore gives the explicit robust conditions

$$
\boxed{0<m<N,\qquad
\sigma<\frac{s}{8\max(m/N,1-m/N)}.}
$$

Starting from the specified pure habitats, the populations then remain in $x\ge3/4$, $y\le1/4$. Their global frequency lies between $3q/4$ and $q+(1-q)/4$, so neither [allele](../../../../../../allele.md) fixes. This is a sufficient condition, not a claim that the bound is sharp. If $m=0$ or $m=N$, the population is already fixed; if $\sigma=0$, any mixture of the two pure habitat types persists.

The exactly balanced case illustrates why robustness and the prescribed trajectory differ. When $q=1/2$, symmetry forces $y=1-x$ and

$$
\dot x=(2x-1)[sx(1-x)-\sigma/2].
$$

For $\sigma<s/2$ its heterogeneous limiting state is

$$
x_* =\frac{1+\sqrt{1-2\sigma/s}}2,\qquad y_*=1-x_*.
$$

Here $f'(x_*)=f'(y_*)=-s+3\sigma$, so the full [Jacobian matrix](../../../../../../jacobian-matrix.md) has diagonal entries $f'(x_*)-\sigma/2$ and off-diagonal entries $\sigma/2$. Its two full-system [eigenvalues](../../../../../../eigenvalue.md) are $-s+3\sigma$ and $-s+2\sigma$: the [symmetric underdominant two-cluster equilibrium](../../../../../../symmetric-underdominant-two-cluster-equilibrium.md) is robustly attracting only for $\sigma<s/3$. For larger migration the exactly symmetric initial condition can still avoid fixation, eventually approaching the spatially uniform frequency $1/2$ when $\sigma\ge s/2$, but the symmetry-broken mean-frequency mode is unstable. A finite population with [genetic drift](../../../../../../genetic-drift.md) need not maintain deterministic coexistence indefinitely.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
