<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal Rg(s,\omega)$ be the [Radon transform](../../../../../../radon-transform.md)

$$
\mathcal Rg(s,\omega)=\int_{y\cdot\omega=s}g(y)\,dA_y.
$$

Taking the large-radius limit in the Kirchhoff formula, with $\xi=t-r$ fixed for the outgoing limit and $\eta=t+r$ fixed for the incoming limit, gives the [radiation fields](../../../../../../radiation-field.md)

$$
\psi_+(\xi,\omega)
=\frac1{4\pi}
\left[
\mathcal Ru_1(-\xi,\omega)
-\partial_s\mathcal Ru_0(-\xi,\omega)
\right],
$$



$$
\psi_-(\eta,\omega)
=-\frac1{4\pi}
\left[
\mathcal Ru_1(\eta,\omega)
+\partial_s\mathcal Ru_0(\eta,\omega)
\right].
$$

Indeed, the expanding spheres converge after multiplication by $r/t$ to the planes $y\cdot\omega=-\xi$ and $y\cdot\omega=\eta$, respectively.

The Radon transforms of smooth compactly supported functions are smooth. If the data are supported in a ball of radius $R$, these transforms vanish for $|s|>R$. Hence both radiation fields are well-defined smooth functions of compact support in the null-time variable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
