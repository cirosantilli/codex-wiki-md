<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the objective as $F_a(x)=\alpha x^2/2+n^{-1}\sum_i\ell_i(x)$ with $\ell_i(x)=\max\{0,1-a_ix\}$. Each [hinge loss](../../../../../../hinge-loss.md) is finite and convex, so the [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) applies without a qualification gap. Its [subdifferential](../../../../../../subdifferential.md) is

$$
\partial\ell_i(x)=
\begin{cases}
\{-a_i\},&1-a_ix>0,\\
\{0\},&1-a_ix<0,\\
\{-\lambda_i a_i:0\leq\lambda_i\leq1\},&1-a_ix=0.
\end{cases}
$$

This formula also covers $a_i=0$, if such a sample is allowed, because the loss is then constant. For a [convex function](../../../../../../convex-function.md), zero in the [subdifferential](../../../../../../subdifferential.md) is necessary and sufficient for global optimality. Thus **$x$ is optimal exactly when** there are weights $\lambda_i$ such that

$$
\boxed{\alpha x=\frac1n\sum_{i=1}^n\lambda_i a_i,\qquad
\lambda_i=
\begin{cases}
1,&a_ix<1,\\
0,&a_ix>1,\\
\text{any value in }[0,1],&a_ix=1.
\end{cases}}
$$

Equivalently, using $I(x)=\{i:a_ix<1\}$ and $J(x)=\{i:a_ix=1\}$,

$$
\alpha nx\in\sum_{i\in I(x)}a_i+\sum_{i\in J(x)}[0,1]a_i.
$$

The notation $[0,1]a_i$ denotes the segment between $0$ and $a_i$, also when $a_i<0$. This avoids reversing interval endpoints for negative-class samples.

Because $\alpha>0$, the objective is [strongly convex](../../../../../../strongly-convex-function.md), and $F_a(x)\geq\alpha x^2/2$ makes it coercive. It is continuous, so a minimizer exists and is unique for every finite data vector $a$. The weights at exact margins need not be unique even though $x$ is. These are the [hinge-loss optimality weights](../../../../../../hinge-loss-optimality-weight.md) for the one-dimensional [support vector machine](../../../../../../support-vector-machine.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
