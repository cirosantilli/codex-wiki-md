<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For admissible initial data, for example a [square-integrable function](../../../../../../square-integrable-function.md) on the interval, expand in the sine [eigenfunctions](../../../../../../eigenfunction.md) of the Dirichlet [Laplacian](../../../../../../laplacian.md):

$$
u(x,0)=\sum_{j\ge1}c_j\sin(j\pi x),\qquad
u(x,t)=\sum_{j\ge1}c_j e^{(\kappa-j^2\pi^2)t}\sin(j\pi x).
$$

The expansion follows either from [separation of variables](../../../../../../separation-of-variables.md) or the complete sine [orthogonal basis](../../../../../../orthogonal-basis.md). If $\kappa<\pi^2$, every growth rate is negative and [Parseval's identity](../../../../../../parseval-identity.md) gives

$$
\|u(\cdot,t)\|_{L^2}^2=\frac12\sum_{j\ge1}|c_j|^2e^{2(\kappa-j^2\pi^2)t}
\le e^{-2(\pi^2-\kappa)t}\|u(\cdot,0)\|_{L^2}^2.
$$

Thus all finite-energy data decay. The convergence is also uniform in $x$ after any fixed positive time: apply [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to the sine series, using the summable factors $e^{-2(j^2-1)\pi^2t}$, to bound its supremum by a constant times $e^{-(\pi^2-\kappa)t}$ for $t\ge t_0>0$.

Conversely choose $u(x,0)=\sin\pi x$. Then $u(x,t)=e^{(\kappa-\pi^2)t}\sin\pi x$, which is stationary at equality and grows when $\kappa>\pi^2$. **All initial conditions decay if and only if $\kappa<\pi^2$.** This is the continuous part of the [reaction-diffusion spectral decay threshold](../../../../../../reaction-diffusion-spectral-decay-threshold.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
