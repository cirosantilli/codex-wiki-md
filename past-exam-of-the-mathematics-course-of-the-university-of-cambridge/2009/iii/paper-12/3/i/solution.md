<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d=\operatorname{dist}(\Omega',\partial\Omega)>0$. Choose a [smooth cutoff function](../../../../../../smooth-cutoff-function.md) $\eta\in C_c^\infty(\Omega)$ with $0\leq\eta\leq1$, $\eta=1$ on $\Omega'$ and $|D\eta|\leq C(n)/d$. Such cutoffs can be constructed by mollifying the indicator of a fixed small neighbourhood of $\overline{\Omega'}$. Write $M=\|A\|_{\infty,\mathrm{op}}$, $B=\|b\|_\infty$ and $C_0=\|c\|_\infty$; these are controlled by the individual coefficient bounds and dimension.

The [weak formulation](../../../../../../weak-formulation.md), extended to [compactly supported](../../../../../../compact-support.md) $H^1$ tests by density, is

$$
\int_\Omega A Du\cdot D\varphi-\int_\Omega(b\cdot Du+cu)\varphi=-\int_\Omega f\varphi.
$$

We may use $\varphi=\eta^2u$, since $u\in H^1_{\mathrm{loc}}$. Expanding its [gradient](../../../../../../gradient.md) and using [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) gives

$$
\lambda\int\eta^2|Du|^2\leq2M\int\eta|u||Du||D\eta|+B\int\eta^2|u||Du|+C_0\int\eta^2u^2+\int\eta^2|fu|.
$$

Apply [Young inequality](../../../../../../young-s-inequality-for-products.md) to the first two terms, allocating at most $\lambda/4$ of the [gradient](../../../../../../gradient.md) integral to each. Bound $|fu|\leq(f^2+u^2)/2$ in the last term. Absorbing those [gradient](../../../../../../gradient.md) contributions yields the [Caccioppoli inequality with bounded lower-order terms](../../../../../../caccioppoli-inequality-with-bounded-lower-order-terms.md)

$$
\int\eta^2|Du|^2\leq C(n,\lambda,M,B,C_0)\left[\int(1+|D\eta|^2)u^2+\int\eta^2f^2\right].
$$

Consequently $\|Du\|_{L^2(\Omega')}\leq C(\|u\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)})$. Adding the $L^2$ [norm](../../../../../../norm.md) of $u$ proves

$$
\boxed{\|u\|_{W^{1,2}(\Omega')}\leq C\left(\|u\|_{L^2(\Omega)}+\|f\|_{L^2(\Omega)}\right),}
$$

where $C$ has precisely the stated dependence on dimension, ellipticity, coefficient bounds and $d$. The proof uses $|c|$, so no sign condition on the zeroth-order term is required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
