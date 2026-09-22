<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Evaluate the metric [inner products](../../../../../../inner-product.md) of the proposed [orthonormal tetrad](../../../../../../orthonormal-frame-in-spacetime.md) to first order in the [vector cosmological perturbation](../../../../../../vector-cosmological-perturbation.md):

$$
\begin{aligned}
g(E_0,E_0)&=-1,\\
g(E_0,E_i)&=a^{-2}(g_{00}B_i+g_{0i})=-B_i+B_i=0,\\
g(E_i,E_j)&=a^{-2}(g_{ij}+B_i g_{0j}+B_j g_{i0}+B_iB_jg_{00})=\delta_{ij}+O(B^2).
\end{aligned}
$$

The [orthonormal tetrad](../../../../../../orthonormal-frame-in-spacetime.md) therefore has [metric signature](../../../../../../metric-signature.md) $(-,+,+,+)$ to the required order. Put $q=\epsilon/a^2$ and $b=\mathbf e\cdot\mathbf B$. The [photon](../../../../../../photon.md) momentum components are

$$
p^0=q(1+b),\qquad p^i=qe^i.
$$

They satisfy the [null vector](../../../../../../null-vector.md) condition to first order, with $|\mathbf e|=1$.

Use $\eta$ as parameter in the time component of the [geodesic equation](../../../../../../geodesic-equation.md):

$$
\frac{dp^0}{d\eta}+\Gamma^0_{\alpha\beta}\frac{p^\alpha p^\beta}{p^0}=0.
$$

The derivative of the direction is first order, since the background [photon](../../../../../../photon.md) moves on a straight comoving line; $B_i\,de^i/d\eta$ is consequently second order. With $d\mathbf x/d\eta=\mathbf e+O(B)$,

$$
\frac1q\frac{dp^0}{d\eta}=\left(\frac{\epsilon'}\epsilon-2\mathcal H\right)(1+b)+e^i\dot B_i+e^ie^j\partial_jB_i+O(B^2).
$$

The supplied [Levi-Civita connection](../../../../../../levi-civita-connection.md) coefficients give

$$
\frac1q\Gamma^0_{\alpha\beta}\frac{p^\alpha p^\beta}{p^0}=2\mathcal H(1+b)-e^ie^j\partial_jB_i+O(B^2).
$$

The spatial gradients and all background expansion terms cancel. Since $\epsilon'/\epsilon$ vanishes in the background, its product with $b$ is also second order. The [photon energy redshift from a vector metric perturbation](../../../../../../photon-energy-redshift-from-a-vector-metric-perturbation.md) is therefore

$$
\boxed{\frac{d\ln\epsilon}{d\eta}+e^i\dot B_i=0.}
$$

An independent check uses the covariant component $p_0=g_{0\mu}p^\mu=-\epsilon+O(B^2)$. The covariant [geodesic equation](../../../../../../geodesic-equation.md) gives $dp_0/d\eta=(2p^0)^{-1}\partial_\eta g_{\alpha\beta}p^\alpha p^\beta=\epsilon e^i\dot B_i$; the conformal expansion term vanishes by the [null vector](../../../../../../null-vector.md) condition and reproduces the same result.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
