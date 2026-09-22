<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $V_0=\Delta U/2$, $z_\pm=\pm h/2$, $B=g\Delta\rho/(2\rho_0)$ and $d=B/(2k)$. The velocity is linear through all three layers, so $U(z_\pm)=\pm V_0$ and $U'$ has no jump. Each interface has density drop $\Delta\rho/2$. The [jump conditions for stratified inviscid shear flow](../../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) become

$$
[\widehat w]=0,\qquad [\widehat w']=-\frac{B}{(U(z_\pm)-c)^2}\widehat w(z_\pm).
$$

Between interfaces, the [Taylor–Goldstein equation](../../../../../../../taylor-goldstein-equation.md) is $\widehat w''-k^2\widehat w=0$. A decaying solution can therefore be written

$$
\widehat w(z)=b_+e^{-k|z-z_+|}+b_-e^{-k|z-z_-|}.
$$

Its derivative jumps are $-2kb_\pm$, while its values at the interfaces are $b_\pm+e^{-kh}b_\mp$. Hence the coefficients satisfy

$$
\begin{pmatrix}(V_0-c)^2-d&-de^{-kh}\\-de^{-kh}&(-V_0-c)^2-d\end{pmatrix}\begin{pmatrix}b_+\\b_-\end{pmatrix}=0.
$$

The determinant must vanish. With $\widetilde c=c/V_0$, $\alpha=kh/2$ and $J=g\Delta\rho h/(\rho_0\Delta U^2)$, one has $d/V_0^2=J/(2\alpha)$. Expanding gives the [dispersion relation for two density interfaces in uniform shear](../../../../../../../dispersion-relation-for-two-density-interfaces-in-uniform-shear.md):

$$
\boxed{\widetilde c^4-\left(2+\frac J\alpha\right)\widetilde c^2+\frac{(2\alpha-J)^2-J^2e^{-4\alpha}}{4\alpha^2}=0.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
