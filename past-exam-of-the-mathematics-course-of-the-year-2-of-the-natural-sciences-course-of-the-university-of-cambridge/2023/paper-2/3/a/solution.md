<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [product rule](../../../../../product-rule.md) to the [vector field](../../../../../vector-field.md) $\Phi\nabla\Psi-\Psi\nabla\Phi$:

$$
\nabla\cdot(\Phi\nabla\Psi-\Psi\nabla\Phi)
=\Phi\Delta\Psi-\Psi\Delta\Phi.
$$

The gradient cross terms cancel. Integrating and applying the [divergence theorem](../../../../../divergence-theorem.md) with outward unit normal $\mathbf n$ proves [Green's second identity](../../../../../green-second-identity.md):

$$
\boxed{\int_V(\Phi\Delta\Psi-\Psi\Delta\Phi)\,dV
=\oint_S(\Phi\partial_n\Psi-\Psi\partial_n\Phi)\,dS.}
$$

Choose the [Dirichlet Green function](../../../../../dirichlet-green-function.md) $G_D(\mathbf r,\mathbf r')$ with $\Delta_{\mathbf r}G_D=\delta(\mathbf r-\mathbf r')$ and $G_D=0$ on $S$. Taking $\Psi=G_D$ and using the [Dirac delta distribution](../../../../../dirac-delta-function.md), the left side becomes $\Phi(\mathbf r')$ while the second boundary term vanishes. Hence

$$
\boxed{\Phi(\mathbf r')=\oint_S f(\mathbf r)\,\partial_{n_{\mathbf r}}G_D(\mathbf r,\mathbf r')\,dS.}
$$

The plus sign is tied to the convention $\Delta G_D=+\delta$, whose free-space [fundamental solution](../../../../../fundamental-solution-of-a-linear-differential-operator.md) is negative in three dimensions. The singularity may equivalently be handled by excising a small sphere about $\mathbf r'$ before applying the smooth identity.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
