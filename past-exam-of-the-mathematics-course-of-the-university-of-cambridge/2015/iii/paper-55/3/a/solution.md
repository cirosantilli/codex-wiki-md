<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Newtonian gauge](../../../../../../newtonian-gauge.md), the coordinate-comoving observer has normalized four-velocity $u^\mu=a^{-1}(1-\psi,\mathbf0)$, hence $u_0=a(1+\psi)$. In the $(+---)$ convention the measured photon energy is $E=u_\mu p^\mu$. Thus **to first order**

$$
\boxed{E=a(1+\psi)\frac\epsilon{a^2}(1-\psi)=\frac\epsilon a+O(\psi^2).}
$$

Use the time component of the [geodesic equation](../../../../../../geodesic-equation.md) and divide by $p^0=d\eta/d\lambda$:

$$
\frac{dp^0}{d\eta}=-\Gamma^0{}_{\alpha\beta}\frac{p^\alpha p^\beta}{p^0}.
$$

Let $\mathcal H=a'/a$ and take the photon path direction $\mathbf e$ at zeroth order. The left side divided by $\epsilon/a^2$ is $\epsilon'/\epsilon-2\mathcal H+2\mathcal H\psi-d\psi/d\eta$. The contraction on the right side, using the provided connection coefficients, is

$$
-2\mathcal H+2\mathcal H\psi-\partial_\eta\psi
-2\mathbf e\cdot\nabla\psi+\partial_\eta\phi.
$$

The homogeneous expansion cancels. Therefore **the scalar photon energy-redshift law is**

$$
\boxed{\frac{d\ln\epsilon}{d\eta}=\partial_\eta\phi-\mathbf e\cdot\nabla\psi
=-\frac{d\psi}{d\eta}+\partial_\eta\phi+\partial_\eta\psi.}
$$

The total derivative is $d/d\eta=\partial_\eta+\mathbf e\cdot\nabla$ on the unperturbed ray. Perturbing that path inside a first-order potential would contribute only at second order. The homogeneous $a^{-1}$ energy redshift is already removed by the comoving momentum variable $\epsilon$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
