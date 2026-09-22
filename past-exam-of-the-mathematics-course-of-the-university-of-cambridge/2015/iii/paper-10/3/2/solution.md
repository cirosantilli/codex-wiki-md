<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We use the homogeneous version of the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) in three dimensions:

$$
\|h\|_{L^6(\mathbb R^3)}\leq C_S\|\nabla h\|_{L^2(\mathbb R^3)},\qquad h\in\dot H^1(\mathbb R^3).
$$

Here [homogeneous Sobolev space](../../../../../../homogeneous-sobolev-space.md) $\dot H^1$ is the completion of compactly supported [smooth functions](../../../../../../smooth-function.md) in the [L2 norm](../../../../../../l2-norm.md) of the [gradient](../../../../../../gradient.md), identified with its $L^6$ representative. Apply this [Sobolev inequality](../../../../../../sobolev-inequality.md) both to $\phi$ and to its [spatial derivatives](../../../../../../spatial-derivative.md).

Let

$$
B(t)=\left(\sum_{i=1}^3\|\partial_i\phi_t(t)\|_2^2+
\sum_{i,j=1}^3\|\partial_i\partial_j\phi(t)\|_2^2\right)^{1/2}.
$$

The [Plancherel theorem](../../../../../../plancherel-theorem.md) identifies the [L2 norm](../../../../../../l2-norm.md) of the [Hessian matrix](../../../../../../hessian-matrix.md) with $\|\phi\|_{\dot H^2}$, because $\sum_{i,j}\xi_i^2\xi_j^2=|\xi|^4$. In particular,

$$
\|\phi\|_{\dot H^2}+\|\phi_t\|_{\dot H^1}\leq\sqrt2 B(t),\qquad B(0)\leq D.
$$

Differentiating the [defocusing semilinear wave equation](../../../../../../defocusing-semilinear-wave-equation.md) gives $\Box(\partial_i\phi)=3\phi^2\partial_i\phi$. By the [Holder inequality](../../../../../../holder-inequality.md) with exponents $3$ and $6$, the preceding [Sobolev inequality](../../../../../../sobolev-inequality.md), and conservation of the positive [wave energy](../../../../../../wave-energy.md),

$$
\begin{aligned}
\|\phi^2\nabla\phi\|_2
&\leq\|\phi\|_6^2\|\nabla\phi\|_6\\
&\leq C\|\nabla\phi\|_2^2\|D_x^2\phi\|_2
\leq 2CE B(t).
\end{aligned}
$$

Use the inhomogeneous [wave energy estimate](../../../../../../wave-energy-estimate.md) simultaneously for the three [spatial derivatives](../../../../../../spatial-derivative.md). It gives

$$
B(t)\leq B(0)+C E\int_0^t B(s)\,ds.
$$

The [Gronwall inequality](../../../../../../gronwall-inequality.md) therefore yields $B(t)\leq D\exp(C E t)$. We may take the continuous, locally bounded function

$$
\boxed{f(T)=\sqrt2 D\exp(C E T).}
$$

The constant is universal; the dependence on the initial data is only through $D$ and $E$. The [H2 bound for the defocusing cubic wave equation](../../../../../../h2-bound-for-the-defocusing-cubic-wave-equation.md) holds on every existing smooth interval, without assuming the global conclusion. If $D=0$ or $E=0$, the zero solution satisfies the same estimate.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
