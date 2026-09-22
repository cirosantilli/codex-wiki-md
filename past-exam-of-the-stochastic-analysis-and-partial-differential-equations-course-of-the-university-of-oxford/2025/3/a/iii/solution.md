<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A second-order [nondivergence-form elliptic operator](../../../../../nondivergence-form-elliptic-operator.md) on a domain $D\subseteq\mathbb R^d$ has the form

$$
\mathcal Af(x)=\sum_{j,k=1}^d a_{jk}(x)\partial_{jk}f(x)
+\sum_{j=1}^db_j(x)\partial_jf(x)+c(x)f(x).
$$

Only the symmetric part of $a$ affects the [Hessian matrix](../../../../../hessian-matrix.md) term, so one may take $a(x)$ symmetric. The operator is a [uniformly elliptic operator](../../../../../uniformly-elliptic-operator.md) if there is a constant $\kappa>0$, independent of $x$, such that

$$
\boxed{\sum_{j,k=1}^da_{jk}(x)\xi_j\xi_k\geq\kappa|\xi|^2
\qquad(x\in D,\ \xi\in\mathbb R^d).}
$$

A common bounded-coefficient convention additionally requires an upper bound $\sum a_{jk}(x)\xi_j\xi_k\leq\Lambda|\xi|^2$ with $\Lambda<\infty$. The lower bound says that the principal [quadratic form](../../../../../quadratic-form-split.md) cannot degenerate in any direction or at any location.

For an explicit stochastic example, standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) has [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md)

$$
\boxed{\mathcal A=\tfrac12\Delta,\qquad a_{jk}=\tfrac12\delta_{jk},\quad b=0,\quad c=0.}
$$

Its principal [quadratic form](../../../../../quadratic-form-split.md) is $|\xi|^2/2$, so it is [uniformly elliptic](../../../../../uniformly-elliptic-operator.md) with $\kappa=\Lambda=1/2$. More generally, a sufficiently regular [stochastic differential equation](../../../../../stochastic-differential-equation.md) $dX_t=b(X_t)\,dt+\Sigma(X_t)\,dB_t$ has [diffusion generator](../../../../../diffusion-generator.md) $b\cdot\nabla+\tfrac12(\Sigma\Sigma^{\mathsf T}):D^2$; it is [uniformly elliptic](../../../../../uniformly-elliptic-operator.md) when $\Sigma\Sigma^{\mathsf T}$ has a uniformly positive lower bound. A conservative [diffusion process](../../../../../markov-diffusion.md) has no zeroth-order term, since its [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) annihilates constants.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
