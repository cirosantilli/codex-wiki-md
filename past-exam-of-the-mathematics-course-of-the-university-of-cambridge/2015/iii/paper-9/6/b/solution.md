<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $x$ with $\operatorname{dist}(x,\partial\Omega)>\sigma$ and use $\eta_x(y)=\phi_\sigma(x-y)$ as the [test function](../../../../../../test-function.md) in part (a). Its support lies compactly inside $\Omega$. Differentiating the [convolution](../../../../../../convolution.md) under the integral is allowed, and $D_{y_i}\eta_x=-D_{x_i}\phi_\sigma(x-y)$ while $\Delta_y\eta_x=\Delta_x\phi_\sigma(x-y)$. Consequently

$$
\begin{aligned}
\Delta u_\sigma(x)&=\int_\Omega u(y)\Delta_y\eta_x(y)\,dy\\
&=-\sum_i\int_\Omega b^i(y)u(y)D_{y_i}\eta_x(y)\,dy+\int_\Omega(cu+f)(y)\eta_x(y)\,dy\\
&=\sum_iD_{x_i}\int_\Omega b^i(y)u(y)\phi_\sigma(x-y)\,dy+(cu)_\sigma(x)+f_\sigma(x).
\end{aligned}
$$

Thus

$$
\boxed{\Delta u_\sigma=\sum_iD_i(b^iu)_\sigma+(cu)_\sigma+f_\sigma}
$$

at every stated interior point. This is the [convolution derivative identity](../../../../../../differentiation-commutes-with-convolution.md). The [convolutions](../../../../../../convolution.md) are local, so no integrability of the smooth coefficients all the way to the boundary is needed. In particular, $(b^iu)_\sigma$ is the [convolution](../../../../../../convolution.md) of the product; it must not be replaced by $b^iu_\sigma$ for a variable coefficient.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
