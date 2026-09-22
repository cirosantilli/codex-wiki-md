<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the scattering-potential convention $V(\mathbf r)=k^2[n(\mathbf r)^2-1]$. Let $G_k(\mathbf r,\mathbf r')=e^{ik|\mathbf r-\mathbf r'|}/(4\pi|\mathbf r-\mathbf r'|)$, so $(\Delta+k^2)G_k=-\delta$. Since $(\Delta+k^2)\psi=-V\psi$, the outgoing Green representation is the [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md)

$$
\psi=\psi_i+T\psi,\qquad (Tf)(\mathbf r)=\int_DG_k(\mathbf r,\mathbf r')V(\mathbf r')f(\mathbf r')d\mathbf r'.
$$

Iterating it produces the [Born series](../../../../../../born-series.md)

$$
\boxed{\psi_s=\sum_{j=1}^\infty T^j\psi_i.}
$$

For example its first two terms are

$$
\psi_s^{[1]}(\mathbf r)=\int_DG_k(\mathbf r,\mathbf r_1)V(\mathbf r_1)\psi_i(\mathbf r_1)d\mathbf r_1,
$$



$$
\psi_s^{[2]}(\mathbf r)=\int_D\int_DG_k(\mathbf r,\mathbf r_2)V(\mathbf r_2)G_k(\mathbf r_2,\mathbf r_1)V(\mathbf r_1)\psi_i(\mathbf r_1)d\mathbf r_1d\mathbf r_2.
$$

The first term describes one scattering event driven by the incident field. The second propagates its first scattered wave to another interaction before reaching the observer. Higher terms contain more successive interactions, including repeated visits to the same region; they account for multiple scattering rather than additional incident waves.

A sufficient convergence condition on an appropriate field [norm](../../../../../../norm.md) is $\|T\|=\rho<1$. Then the first-Born remainder is bounded by $\rho^2\|\psi_i\|/(1-\rho)$, while $\|T\psi_i\|\le\rho\|\psi_i\|$. A simple concrete sufficient condition on the bounded scatterer, using the supremum [norm](../../../../../../norm.md), is

$$
\sup_{\mathbf r\in D}\int_D|G_k(\mathbf r,\mathbf r')V(\mathbf r')|d\mathbf r'\ll1.
$$

This makes the field inside the inhomogeneity close to the incident field. Physically weak index contrast with small accumulated phase shift, such as $k\ell|n-1|\ll1$ for a smooth weak scatterer of thickness $\ell$, is a common first-Born regime, provided resonant enhancement and multiple reflections are negligible. Weak local contrast alone is not sufficient for an arbitrarily thick scatterer. If the opposite sign convention for $V$ is used, the [integral](../../../../../../integral.md) operator changes sign and the same consistent iteration applies.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
