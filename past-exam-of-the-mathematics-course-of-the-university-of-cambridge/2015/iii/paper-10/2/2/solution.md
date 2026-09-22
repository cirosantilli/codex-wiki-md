<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We establish a quantitative [almost global existence for wave equations](../../../../../../almost-global-existence-for-wave-equations.md) estimate. Take $0<\varepsilon\leq1$, fix an integer $m\geq6$, and use the [commutation vector fields for the wave equation](../../../../../../commutation-vector-field-for-the-wave-equation.md) from the preceding part. Put $\partial=(\partial_t,\nabla)$ and define the [commuted wave energy](../../../../../../commuted-wave-energy.md)

$$
A_m(t)=\sum_{|I|\leq m}\|\partial Z^I\phi(t)\|_2.
$$

All these [L2 norms](../../../../../../l2-norm.md) are finite on any smooth existence interval by [finite propagation speed](../../../../../../finite-propagation-speed.md). At $t=0$, the polynomial coefficients of the [vector fields](../../../../../../vector-field.md) are bounded on the fixed [compact support](../../../../../../compact-support.md) of the [Cauchy data](../../../../../../cauchy-data.md). Whenever a higher time derivative occurs, use $\phi_{tt}=\Delta\phi-\phi_t^2$ and its differentiated versions to express it in terms of initial spatial derivatives. Every term contains at least one factor of $\varepsilon$; consequently

$$
A_m(0)\leq C_0\varepsilon
$$

for a constant depending only on finitely many derivatives and the [support](../../../../../../support.md) radius of $\phi_0,\phi_1$.

The [commutators](../../../../../../commutator.md) $[Z,\partial_\mu]$ are constant linear combinations of translations. Together with $[\Box,S]=2\Box$ and the [Leibniz rule](../../../../../../leibniz-rule.md), this shows that each commuted source is a finite linear combination of products

$$
\partial_\mu Z^J\phi\,\partial_\nu Z^K\phi,\qquad |J|+|K|\leq |I|.
$$

This statement includes the extra copies of the original source produced by the [scaling vector field](../../../../../../scaling-vector-field.md). In each product put the factor with fewer commutations in the [Lp norm](../../../../../../lp-norm.md) $L^\infty$ and the other in the [L2 norm](../../../../../../l2-norm.md). The lower order is at most $\lfloor m/2\rfloor$. Applying the [Klainerman-Sobolev inequality](../../../../../../klainerman-sobolev-inequality.md) to $\partial_\mu Z^J\phi$ costs at most two additional commutations; commuting those past $\partial_\mu$ introduces only lower-order translations. Since $\lfloor m/2\rfloor+2\leq m$,

$$
\sum_{|I|\leq m}\|\Box Z^I\phi(t)\|_2\leq\frac{C_m}{1+t}A_m(t)^2.
$$

The inhomogeneous [wave energy estimate](../../../../../../wave-energy-estimate.md) now gives

$$
A_m(t)\leq C_0\varepsilon+C_m\int_0^t\frac{A_m(s)^2}{1+s}\,ds.
$$

Let $T_\varepsilon=\varepsilon^{-N}$. Use a [bootstrap argument](../../../../../../bootstrap-argument.md) with $A_m(t)\leq2C_0\varepsilon$ up to the smaller of $T_\varepsilon$ and the maximal existence time. The [energy estimate](../../../../../../energy-estimate.md) improves this to

$$
A_m(t)\leq C_0\varepsilon+4C_mC_0^2\varepsilon^2\log(1+T_\varepsilon).
$$

For each fixed $N$,

$$
\varepsilon\log(1+\varepsilon^{-N})\longrightarrow0\quad\text{as}\quad\varepsilon\downarrow0.
$$

Choose $\varepsilon_N\leq1$ so that $4C_mC_0\varepsilon\log(1+\varepsilon^{-N})\leq1/2$ for every $0<\varepsilon\leq\varepsilon_N$. Then $A_m(t)\leq(3/2)C_0\varepsilon$, a strict improvement. A [continuity](../../../../../../continuous-function.md) argument closes the [bootstrap argument](../../../../../../bootstrap-argument.md).

Finally, the translation terms in $A_m$ control ordinary spatial [Sobolev norms](../../../../../../sobolev-norm.md) of $\partial\phi$. The missing [L2 norm](../../../../../../l2-norm.md) of $\phi$ satisfies

$$
\|\phi(t)\|_2\leq\varepsilon\|\phi_0\|_2+\int_0^t\|\phi_t(s)\|_2\,ds.
$$

Thus the full local-existence [Sobolev norms](../../../../../../sobolev-norm.md) remain bounded on this finite interval. The [smooth continuation criterion for semilinear wave equations](../../../../../../smooth-continuation-criterion-for-semilinear-wave-equations.md) extends the solution past any finite endpoint before $T_\varepsilon$. To see smooth persistence explicitly, the [tame Sobolev product estimate](../../../../../../tame-sobolev-product-estimate.md) gives $\|\phi_t^2\|_{H^k}\leq C_k\|\phi_t\|_\infty\|\phi_t\|_{H^k}$. Ordinary differentiated [wave energy estimates](../../../../../../wave-energy-estimate.md) therefore bound each higher derivative energy by its initial value times $\exp(C_k\int_0^t\|\phi_t(s)\|_\infty\,ds)$. This is finite on the interval already controlled by the base [commuted wave energy](../../../../../../commuted-wave-energy.md); no separate $\varepsilon_N$ is needed for each derivative order. Therefore

$$
\boxed{\text{the solution is smooth on }[0,\varepsilon^{-N}]\text{ for }0<\varepsilon\leq\varepsilon_N.}
$$

For $\varepsilon=0$ the zero solution is global. The same [energy estimate](../../../../../../energy-estimate.md) in fact permits an exponential lower bound for the lifespan, which is stronger than any fixed inverse power.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
