<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
K(z)=-J\nabla W(z)=(W_y(z),-W_x(z)),\qquad L=\max\left\{1,\sup_z\|D^2W(z)\|_{\mathrm{op}}\right\}.
$$

Symmetry here means $W(-z)=W(z)$, so $\nabla W(0)=0$ and $K(0)=0$. The bounded [Hessian matrix](../../../../hessian-matrix.md) and the fact that $J$ is an [orthogonal matrix](../../../../orthogonal-matrix.md) give

$$
|K(z)-K(z')|\leq L|z-z'|,\qquad |K(z)|\leq L|z|.
$$

Thus the particle system is $\dot X^i=N^{-1}\sum_jK(X^i-X^j)$. On the configuration space with norm $\|X\|_{\max}=\max_i|X^i|$, its vector field has [Lipschitz constant](../../../../lipschitz-constant.md) at most $2L$:

$$
|F_i(X)-F_i(Y)|\leq\frac L N\sum_j\left(|X^i-Y^i|+|X^j-Y^j|\right)\leq2L\|X-Y\|_{\max}.
$$

The [Picard-Lindelöf theorem](../../../../picard-lindelof-theorem.md) gives local existence and uniqueness. Linear growth and the [Gronwall inequality](../../../../gronwall-inequality.md) give $\|X(t)\|_{\max}\leq e^{2Lt}\|X(0)\|_{\max}$, which rules out escape to infinity in finite time and extends the solution to every $t\geq0$.

The associated [empirical measure](../../../../empirical-measure.md) is

$$
\boxed{\mu_t^N=\frac1N\sum_{i=1}^N\delta_{X^i(t)}.}
$$

Here each $\delta_{X^i(t)}$ is a [Dirac measure](../../../../dirac-measure.md). The finite first [absolute moment](../../../../absolute-moment.md) follows from $\int|x|\,d\mu_t^N=N^{-1}\sum_i|X^i(t)|<\infty$. Pairing equal particle labels defines a [coupling](../../../../coupling.md), so

$$
d_1(\mu_t^N,\mu_s^N)\leq\frac1N\sum_i|X^i(t)-X^i(s)|\longrightarrow0\quad(t\to s).
$$

Consequently

$$
\boxed{\mu^N\in C([0,\infty),\mathcal P_1(\mathbb R^2)).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
