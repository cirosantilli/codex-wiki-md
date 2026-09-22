<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the [Radon transform](../../../../../../radon-transform.md) and its transverse [Hilbert transform](../../../../../../hilbert-transform.md) by

$$
Rf(\rho,\theta)=\int_{\mathbb R}F(\tau',\rho,\theta)d\tau',\qquad
Hh(\rho)=\frac1\pi\operatorname{PV}\int_{\mathbb R}\frac{h(\rho')}{\rho-\rho'}d\rho'.
$$

Use the [signed Cauchy boundary operators](../../../../../../signed-cauchy-boundary-operators.md) $P^+=(I+iH)/2$ and $P^-=(-I+iH)/2$. Thus $P^+$ and $-P^-$ are the complementary idempotent projections; $P^-$ itself carries the signed lower-boundary convention. The PDF defines the outside limit $\lambda^-=(1+\varepsilon)e^{i\theta}$ but omits the definition of the inside limit in its displayed formula. We take $\lambda^+=(1-\varepsilon)e^{i\theta}$, as required by that formula.

As $r\to1$, apply the [Sokhotski–Plemelj formula](../../../../../../sokhotski-plemelj-theorem.md) to the kernel from part (b):

$$
\frac1{u+i0v}=\operatorname{PV}\frac1u-i\pi\operatorname{sgn}(v)\delta(u).
$$

The [principal value](../../../../../../cauchy-principal-value.md) contribution is $i\operatorname{sgn}(b_r)HRf/2$. The delta contribution is the same from either side and equals

$$
\frac12\int_{\mathbb R}\operatorname{sgn}(\tau-\tau')F(\tau',\rho,\theta)d\tau'
=\frac12Rf-\int_\tau^\infty F(\tau',\rho,\theta)d\tau'.
$$

Since $b_r<0$ for the inside limit, the resulting **boundary value** is

$$
\boxed{\mu(\lambda^+)=-P^-Rf(\rho,\theta)-\int_\tau^\infty F(\tau',\rho,\theta)d\tau'.}
$$

The outside limit similarly has $P^+Rf$ in place of $-P^-Rf$. Naming the signed convention explicitly prevents a sign error from treating $P^-$ as a positive projection.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
