<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [Interior second-derivative estimate for the Poisson equation](../../../../../../interior-second-derivative-estimate-for-the-poisson-equation.md) using [difference quotients](../../../../../../difference-quotient.md), rather than differentiating the $L^2$ forcing. Fix a coordinate $e_k$ and write $\delta_hv(x)=(v(x+he_k)-v(x))/h$. Choose a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\eta$ equal to one on $\Omega'$ with support compactly contained in $\Omega$, leaving room for all translations with sufficiently small $|h|$. We can arrange $|D\eta|\leq C(n)/d$, where $d=\operatorname{dist}(\Omega',\partial\Omega)$.

The standard difference quotient lemmas give discrete [integration by parts](../../../../../../integration-by-parts.md), $\int a\delta_{-h}b=-\int(\delta_ha)b$, and $\|\delta_hv\|_2\leq\|D_kv\|_2$ on the relevant enlarged set. In the [weak formulation](../../../../../../weak-formulation.md) $\int Du\cdot D\varphi=-\int f\varphi$, use the admissible [test function](../../../../../../test-function.md) $\varphi=-\delta_{-h}(\eta^2\delta_hu)$. Moving a difference quotient onto $Du$ gives

$$
\int\eta^2|D\delta_hu|^2+2\int\eta\delta_hu\,D\delta_hu\cdot D\eta=\int f\,\delta_{-h}(\eta^2\delta_hu).
$$

Set $X=\|\eta D\delta_hu\|_2$ and $Y=\|D\eta\,\delta_hu\|_2$. The cross term has absolute value at most $2XY$. Since $0\leq\eta\leq1$, the difference quotient lemma on the right gives

$$
\left|\int f\,\delta_{-h}(\eta^2\delta_hu)\right|\leq\|f\|_2\|D_k(\eta^2\delta_hu)\|_2\leq\|f\|_2(X+2Y).
$$

The [Young inequality](../../../../../../young-s-inequality-for-products.md) now implies $X^2\leq C(Y^2+\|f\|_2^2)$. Moreover $Y\leq C(n)d^{-1}\|Du\|_{L^2(\Omega)}$, independently of $h$. Hence, for every coordinate $k$,

$$
\|D\delta_hu\|_{L^2(\Omega')}\leq C(n,d)\left(\|Du\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)}\right).
$$

By the [Sobolev characterization by bounded difference quotients](../../../../../../sobolev-characterization-by-bounded-difference-quotients.md), applied to each first [weak derivative](../../../../../../weak-derivative.md) on smaller interior sets, these uniform bounds give all second [weak derivatives](../../../../../../weak-derivative.md). Their bounds pass to the weak limit as $h\to0$. Thus $u\in W^{2,2}_{\mathrm{loc}}(\Omega)$ and

$$
\boxed{\|u\|_{W^{2,2}(\Omega')}\leq C(n,d)\left(\|u\|_{W^{1,2}(\Omega)}+\|f\|_{L^2(\Omega)}\right).}
$$

No derivative of $f$ is used, and no boundary condition is needed for this interior [elliptic regularity](../../../../../../elliptic-regularity.md) argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
