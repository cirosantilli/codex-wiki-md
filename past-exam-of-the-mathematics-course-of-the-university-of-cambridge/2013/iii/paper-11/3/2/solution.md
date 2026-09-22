<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\beta=|H|/M\gg\delta^8$ and $\eta=(\kappa/2)^{1/2}\gg\delta^4$. Choose unit complex numbers $b_h$ so that

$$
T=\mathbb E_x\overline{F(x)}\left(\frac1M\sum_{h\in H}b_hF(x+h)e(-\theta(h)x)\right)\geq\beta\eta
$$

is real and nonnegative. [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md), using $|F|\leq1$, bounds $T^2$ by

$$
\frac1{M^2}\sum_{h,k\in H}b_h\overline{b_k}\,\mathbb E_xF(x+h)\overline{F(x+k)}e(-[\theta(h)-\theta(k)]x).
$$

After setting $y=x+k$, each summand is a unit phase times the [Fourier coefficient on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) of $\partial_{h-k}F$ at frequency $\theta(h)-\theta(k)$.

Let $r(d,\xi)$ count pairs $(h,k)\in H^2$ with $h-k=d$ and $\theta(h)-\theta(k)=\xi$. Grouping terms, another [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) and the [Parseval identity](../../../../../../parseval-identity.md) yield

$$
T^2\leq\frac1{M^2}\left(\sum_{d,\xi}r(d,\xi)^2\right)^{1/2}
\left(\sum_{d,\xi}|\widehat{\partial_dF}(\xi)|^2\right)^{1/2}
\leq\left(\frac{E_\theta(H)}{M^3}\right)^{1/2},
$$

where $E_\theta(H)=\sum r(d,\xi)^2$ is the [additive energy of a frequency graph](../../../../../../additive-energy-of-a-frequency-graph.md). The last inequality uses $\sum_\xi|\widehat{\partial_dF}(\xi)|^2=\mathbb E|\partial_dF|^2\leq1$ for each $d$.

Thus

$$
\boxed{E_\theta(H)\geq(\beta\eta)^4M^3\gg\delta^{48}N^3.}
$$

The bound proves that [derivative correlations force additive frequency energy](../../../../../../derivative-correlations-force-additive-frequency-energy.md). This energy counts exactly the ordered quadruples satisfying the two requested additive relations, after relabelling the difference equality as a sum equality. Shift equalities initially hold modulo $M$, but the shifts lie in $[-N,N]$ and $M>8N$, so they are also integer equalities. Frequency equalities hold in $\mathbb R/\mathbb Z$, as required. Consequently a common exponent **$C=48$** works for both conclusions, after adjusting absolute implicit constants and using $0<\delta\leq1$.

For the [quadratic phase](../../../../../../quadratic-phase.md), the [multiplicative derivative](../../../../../../multiplicative-derivative.md) on the overlap is $\partial_hf_0(x)=e(2\alpha hx+\alpha h^2)$. Hence an explicit choice is

$$
\boxed{\theta(h)=2\alpha h\pmod1.}
$$

Take $|h|\leq\lfloor N/2\rfloor$. The correlation magnitude is $(N-|h|)/M\geq1/32$, and every additive quadruple of shifts satisfies the frequency relation. The interval of shifts has $\gg N^3$ such quadruples by [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md). These particular real frequencies need not belong to the grid used to prove existence for general $f$; evaluating them at the interval's integer coordinates gives the stated exact formula.

A genuinely nonlinear example is the [bracket-linear frequency function](../../../../../../bracket-linear-frequency-function.md)

$$
\boxed{\theta(h)=\sqrt3\,\{\sqrt2\,h\}\pmod1,\qquad H=[-N,N]\cap\mathbb Z.}
$$

It has $\gg N^3$ exact additive quadruples, yet agrees with any affine function $ah+b\pmod1$ at only $o(N)$ shifts, uniformly in the affine function. The question permits giving this example without proof, but the mechanism is useful. For a pair with sum $s$, the value $\lfloor\sqrt2h_1\rfloor+\lfloor\sqrt2h_2\rfloor$ has only two possibilities, $\lfloor\sqrt2s\rfloor$ or $\lfloor\sqrt2s\rfloor-1$. There are $O(N)$ pair classes, so [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) produces $\gg N^3$ collisions with both additive relations.

To see why no long affine agreement occurs, three agreement points force the corresponding lattice points $(h,\lfloor\sqrt2h\rfloor)$ to be collinear: eliminating the affine slope gives $\sqrt3$ times an integer determinant equal to an integer, and irrationality makes that determinant zero. A rational line of slope $p/q$ contains agreement shifts in one residue class modulo $q$, and closeness of $\lfloor\sqrt2h\rfloor$ to $\sqrt2h$ bounds their span by $1/|\sqrt2-p/q|$. Lines with $q$ large have arbitrarily small possible density; for bounded $q$, irrationality of $\sqrt2$ bounds the number uniformly. Thus the maximum agreement is $o(N)$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
