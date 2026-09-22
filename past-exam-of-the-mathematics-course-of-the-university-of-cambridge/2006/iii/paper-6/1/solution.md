<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

First scale the stated unit-ball approximation. For every nonzero residual $r\in F$, apply the hypothesis to $r/\|r\|$ and multiply the resulting vector by $\|r\|$. This gives $v\in E$ with

$$
\|v\|\le R\|r\|,\qquad \|Tv-r\|\le k\|r\|.
$$

For zero residual use $v=0$. Start with $r_0=y$, choose $v_j$ by this rule for $r_j$, and set $r_{j+1}=r_j-Tv_j$. Inductively,

$$
\|r_j\|\le k^j\|y\|,\qquad \|v_j\|\le Rk^j\|y\|.
$$

The [Banach space](../../../../../banach-space-split.md) $E$ therefore contains the sum $x=\sum_{j\ge0}v_j$, with

$$
\boxed{\|x\|\le\frac R{1-k}\|y\|.}
$$

The partial sums satisfy $T\sum_{j=0}^{n-1}v_j=y-r_n$. Boundedness of $T$ gives convergence of the left side to $Tx$, while $r_n\to0$ gives $Tx=y$. Thus **$T$ is [surjective](../../../../../surjective-function.md) with the stated lifting bound**. This [geometric correction for approximate surjectivity](../../../../../geometric-correction-for-approximate-surjectivity.md) used [completeness](../../../../../completeness.md) of $E$, not any unproved [completeness](../../../../../completeness.md) of $F$.

Put $C=R/(1-k)$. Given a [Cauchy sequence](../../../../../cauchy-sequence.md) $(y_n)$ in $F$, choose a subsequence $(y_{n_j})$ such that $\|y_{n_{j+1}}-y_{n_j}\|\le2^{-j}$ for $j\ge1$. Lift each difference to $u_j\in E$ with $Tu_j=y_{n_{j+1}}-y_{n_j}$ and $\|u_j\|\le C2^{-j}$. Lift $y_{n_1}$ to $u_0$. The sum $u=u_0+\sum_{j\ge1}u_j$ exists in $E$, and its image is the limit of the subsequence. A [Cauchy sequence](../../../../../cauchy-sequence.md) with a convergent subsequence converges to the same limit: use the [triangle inequality](../../../../../triangle-inequality.md) between an arbitrary late term, a later subsequence term, and the limit. This proves **$F$ is complete**, the [completeness forced by uniformly bounded lifting](../../../../../completeness-forced-by-uniformly-bounded-lifting.md) principle.

The [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md) states that a bounded [surjective](../../../../../surjective-function.md) linear operator between [Banach spaces](../../../../../banach-space-split.md) maps open sets to open sets. In particular a bounded linear bijection between [Banach spaces](../../../../../banach-space-split.md) has a bounded inverse. To deduce the [closed graph theorem](../../../../../closed-graph-theorem.md), let $S:E_1\to F_1$ be an everywhere-defined [linear map](../../../../../linear-map.md) between [Banach spaces](../../../../../banach-space-split.md) with closed graph. Its graph is a closed subspace of the Banach product $E_1\times F_1$, with [norm](../../../../../norm.md) $\|(x,y)\|=\|x\|+\|y\|$, so it is itself Banach. The projection

$$
\pi_1:\operatorname{graph}S\to E_1,\qquad(x,Sx)\mapsto x
$$

is a bounded linear bijection. The [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md) makes its inverse bounded. Composing that inverse with the bounded second projection proves that $S$ is bounded. This is the required closed graph conclusion, rather than a continuity assumption on $S$.

Finally consider the identity map $I:(C(X),\|\cdot\|)\to(C(X),\|\cdot\|_\infty)$. If $f_n\to f$ in the new [norm](../../../../../norm.md) and $f_n\to g$ uniformly, each assumed continuous [point evaluation functional](../../../../../point-evaluation-functional.md) gives $f_n(x)\to f(x)$, while [uniform convergence](../../../../../uniform-convergence.md) gives $f_n(x)\to g(x)$. Hence $f=g$. Since both spaces are metric, this sequential argument proves the graph is closed. Both [norms](../../../../../norm.md) are complete, so the [closed graph theorem](../../../../../closed-graph-theorem.md) makes $I$ bounded. Its inverse is bounded by the [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md). Consequently there are constants $c,C'>0$ such that

$$
\boxed{c\|f\|_\infty\le\|f\|\le C'\|f\|_\infty\qquad(f\in C(X)).}
$$

This proves [Banach norm rigidity from continuous point evaluations](../../../../../banach-norm-rigidity-from-continuous-point-evaluations.md). Pointwise continuity alone would not give a common bound on all evaluations; [completeness](../../../../../completeness.md) supplies that through the closed graph argument.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
