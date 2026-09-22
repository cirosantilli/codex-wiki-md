<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) is a family of continuous maps $R_\alpha:\mathcal V\to\mathcal U$, $\alpha>0$, such that

$$
R_\alpha f\longrightarrow A^\dagger f\qquad(\alpha\downarrow0)
$$

for every $f$ in the domain of the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md). A linear regularization has each $R_\alpha$ bounded and linear. For example, [Tikhonov regularization](../../../../../../tikhonov-regularization.md) gives

$$
R_\alpha=(A^*A+\alpha I)^{-1}A^*.
$$

A nonlinear example is [quartic-norm variational regularization](../../../../../../quartic-norm-variational-regularization.md):

$$
R_\alpha f=\arg\min_u\left\{\|Au-f\|^2+\alpha\|u\|^4\right\}.
$$

Its strictly convex norm penalty selects the same [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md) as $\alpha\downarrow0$, but the map from data to minimizer is generally nonlinear.

A [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md) additionally has a parameter rule $\alpha(\delta,f_\delta)>0$ such that, for every admissible exact $f$,

$$
\boxed{\sup_{\|f_\delta-f\|\leq\delta}
\|R_{\alpha(\delta,f_\delta)}f_\delta-A^\dagger f\|\longrightarrow0
\quad(\delta\downarrow0).}
$$

An [a priori regularization parameter choice](../../../../../../a-priori-regularization-parameter-choice.md) depends only on $\delta$ and fixed information about the problem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
