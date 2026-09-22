<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write the nonlinearity as

$$
N(u,v)=(0,u^2).
$$

In one dimension, the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) gives $H^1(\mathbb T)\hookrightarrow L^\infty(\mathbb T)$. Hence

$$
\|u^2-w^2\|_{L^2}
\leq\|u+w\|_{L^\infty}\|u-w\|_{L^2}
\leq C(\|u\|_{H^1}+\|w\|_{H^1})\|u-w\|_{H^1}.
$$

Thus $N:\mathcal H\to\mathcal H$ is locally Lipschitz.

On $C([0,T];\mathcal H)$ define

$$
(\Phi Z)(t)=U(t)Z_0+int_0^tU(t-s)N(Z(s))\,ds.
$$

On a ball of radius $R$, unitarity gives

$$
\|\Phi Z\|_\infty\leq\|Z_0\|_{\mathcal H}+CTR^2,
$$



$$
\|\Phi Z-\Phi W\|_\infty\leq CTR\|Z-W\|_\infty.
$$

Choose $R>\|Z_0\|_{\mathcal H}$ and then $T>0$ small enough that the first bound preserves the ball and $CTR<1$. The [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) gives a unique fixed point. Precisely, the local mild solution is

$$
\boxed{
Z\in C([0,T];\mathcal H),
\qquad
Z(t)=U(t)Z_0+int_0^tU(t-s)(0,u(s)^2)\,ds}.
$$

For general energy data $Z_0\in\mathcal H$, this solution need not be differentiable in $\mathcal H$. If $Z_0\in D(A)=H^2\times H^1$, standard semilinear evolution theory and the smoothness of $N$ give a local classical solution.

The [blow-up alternative for a semilinear evolution equation](../../../../../../blow-up-alternative-for-a-semilinear-evolution-equation.md) says that the solution continues while its $\mathcal H$ norm stays finite, but global existence does not hold for every datum. Spatially constant solutions obey

$$
y''+y=y^2.
$$

For sufficiently large $y(0)>1$ with $y'(0)\geq0$, the solution grows until $y''\geq y^2/2$ and blows up in finite time. These constant functions are periodic and belong to every Sobolev space, so they provide finite-time blow-up examples for the original equation.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
