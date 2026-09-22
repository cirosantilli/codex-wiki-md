<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On the coordinatewise ordered [configuration space](../../../../../mechanical-configuration-space.md), $\mu_1$ stochastically dominates $\mu_2$ when $\int f\,d\mu_1\geq\int f\,d\mu_2$ for every increasing real function $f$. Equivalently, $\mu_1(A)\geq\mu_2(A)$ for every [increasing event](../../../../../increasing-event.md). The [Holley condition](../../../../../holley-condition.md) is the sufficient cross-lattice inequality

$$
\boxed{\mu_1(\omega\vee\eta)\mu_2(\omega\wedge\eta)
\geq\mu_1(\omega)\mu_2(\eta)\quad\text{for all }\omega,\eta.}
$$

Here join and meet are coordinatewise maximum and minimum. This condition implies $\mu_1\geq_{\rm st}\mu_2$ by the [Holley inequality](../../../../../holley-inequality.md); it is not asserted to be necessary. It can be checked on unnormalized weights, since their normalization constants cancel.

Use the weights

$$
b_p(\omega)=p^{o(\omega)}(1-p)^{|E|-o(\omega)},\qquad
r_{p,q}(\omega)=b_p(\omega)q^{k(\omega)}.
$$

For the upper bound, take $\mu_1=\phi_{p,1}$ and $\mu_2=\phi_{p,q}$. Since open-[edge](../../../../../edge-of-a-graph.md) count is modular, the [Bernoulli](../../../../../bernoulli-distribution.md) factors cancel in the Holley ratio, leaving

$$
\frac{b_p(\omega\vee\eta)r_{p,q}(\omega\wedge\eta)}
{b_p(\omega)r_{p,q}(\eta)}
=q^{k(\omega\wedge\eta)-k(\eta)}\geq1.
$$

The last inequality uses $q\geq1$ and the fact that removing [edges](../../../../../edge-of-a-graph.md) cannot reduce the number of components. Thus $\phi_{p,q}\leq_{\rm st}\phi_{p,1}$.

For the lower bound, let $p'=p/[p+q(1-p)]$. Its odds satisfy

$$
\frac{p'}{1-p'}=\frac1q\frac p{1-p}.
$$

Set $a=o(\omega\vee\eta)-o(\omega)=o(\eta)-o(\omega\wedge\eta)$, the number of [edges](../../../../../edge-of-a-graph.md) added to $\omega$ in the union. For $\mu_1=\phi_{p,q}$ and $\mu_2=\phi_{p',1}$, the corresponding ratio is

$$
\frac{r_{p,q}(\omega\vee\eta)b_{p'}(\omega\wedge\eta)}
{r_{p,q}(\omega)b_{p'}(\eta)}
=q^{a+k(\omega\vee\eta)-k(\omega)}\geq1.
$$

Adding one [edge](../../../../../edge-of-a-graph.md) either merges two components or leaves the count unchanged. Therefore adding $a$ [edges](../../../../../edge-of-a-graph.md) reduces $k$ by at most $a$, proving the exponent nonnegative. This also proves the hinted [monotonicity](../../../../../monotonic-function.md) of $k(\omega)+o(\omega)$ rather than assuming it. The [Holley condition](../../../../../holley-condition.md) now proves both [Bernoulli bounds for the random-cluster model](../../../../../bernoulli-bounds-for-the-random-cluster-model.md):

$$
\boxed{\phi_{p',1}\leq_{\rm st}\phi_{p,q}\leq_{\rm st}\phi_{p,1}}.
$$

The same argument holds with wired boundary conditions: identify the wired boundary vertices first and count components on that quotient graph. Taking finite-volume wired limits preserves every increasing cylinder-event inequality. Approximating $\{0\leftrightarrow\infty\}$ by the decreasing events $\{0\leftrightarrow\partial[-n,n]^d\}$ consequently gives

$$
\theta(p',1)\leq\theta^{\rm w}(p,q)\leq\theta(p,1).
$$

Let $a=p_c(1)$. For $p<a$, the upper bound makes the wired [percolation](../../../../../percolation-theory.md) [probability](../../../../../probability.md) zero, so $p_c(q)\geq a$. If $a<1$ and $p'>a$, the lower bound makes it positive. Solving this strict inequality,

$$
\frac p{p+q(1-p)}>a
\quad\Longleftrightarrow\quad
p>\frac{qa}{1+(q-1)a}.
$$

Taking infima proves

$$
\boxed{p_c(1)\leq p_c(q)\leq
\frac{q\,p_c(1)}{1+(q-1)p_c(1)}}.
$$

For $a=1$, the lower bound and the trivial upper bound $p_c(q)\leq1$ give the same conclusion. No assumption about [percolation](../../../../../percolation-theory.md) at the critical parameter is required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
