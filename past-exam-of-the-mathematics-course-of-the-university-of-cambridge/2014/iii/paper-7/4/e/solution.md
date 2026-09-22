<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the correct Gaussian entropy decomposition

$$
 H_N(F)=\int F\log F\,d\mathbf v+\frac N2\log(2\pi)
 +\frac12\int|\mathbf v|^2F\,d\mathbf v.
$$

The last coefficient is $1/2$, as follows from $-\log\gamma_N=N\log(2\pi)/2+|\mathbf v|^2/2$; the printed hint omits it. Under the allowed differentiability and integrability assumptions, the supplied collision invariants conserve mass and energy. Differentiating therefore gives

$$
 \frac d{dt}H_N(F)=N\int(Q-I)F\log F\,d\mathbf v,
$$

where the extra derivative term $\int\partial_tF$ vanishes by [mass conservation](../../../../../../mass-conservation.md). Thus the [Kac entropy production](../../../../../../kac-entropy-production.md) is

$$
 D_N(F)=\frac{N}{2\pi C_N}\sum_{i<j}\int_{\mathbb R^N}\int_0^{2\pi}
 (F-F\circ R_{ij,\theta})\log F\,d\theta\,d\mathbf v.
$$

For one pair, call the double [integral](../../../../../../integral.md) $A_{ij}$. The measure-preserving substitution $(\mathbf v,\theta)\mapsto(R_{ij,\theta}\mathbf v,-\theta)$ interchanges $F$ and $F\circ R_{ij,\theta}$, with angles taken modulo $2\pi$. Averaging the original and substituted expressions gives

$$
 A_{ij}=\frac12\int_{\mathbb R^N}\int_0^{2\pi}
 (F\circ R_{ij,\theta}-F)
 (\log(F\circ R_{ij,\theta})-\log F)\,d\theta\,d\mathbf v.
$$

Since $N/(4\pi C_N)=1/[2\pi(N-1)]$, the desired [Kac entropy dissipation](../../../../../../kac-entropy-production.md) formula is

$$
 \boxed{D_N(F)=\frac1{2\pi(N-1)}\sum_{i<j}\int_{\mathbb R^N}\int_0^{2\pi}
 (F(R_{ij,\theta}\mathbf v)-F(\mathbf v))
 \log\!\frac{F(R_{ij,\theta}\mathbf v)}{F(\mathbf v)}\,d\theta\,d\mathbf v\geq0.}
$$

For positive values $a,b$, $(a-b)(\log a-\log b)\geq0$ because the logarithm is increasing. At two zeros use value zero; at one zero and one positive value use the nonnegative extended value $+\infty$. One may first use positive densities and then regularize by $(F+\varepsilon\gamma_N)/(1+\varepsilon)$; rotation invariance of $\gamma_N$ preserves the formula and permits the usual limit at zeros under the stated assumptions.

Thus **relative entropy is nonincreasing** along the evolution. When the dissipation is finite, zero dissipation means pairwise rotation invariance and hence radiality, by the preceding kernel argument. Radial normalized densities other than $\gamma_N$ can be stationary with positive relative entropy: vanishing dissipation is not a claim that the unique stationary density is Gaussian.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
