<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $w=K^*Kv\in\partial J(u^\dagger)$ from the [normal-operator source condition](../../../../../../normal-operator-source-condition.md), and set $e=u-u^\dagger$. Since $u^\dagger$ is a [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md), the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) gives $K^*(Ku^\dagger-f)=0$. Expand the objective difference and use the [Bregman distance](../../../../../../bregman-divergence.md) definition:

$$
\begin{aligned}
\mathcal F_\alpha(u)-\mathcal F_\alpha(u^\dagger)
&=\frac12\|Ke\|^2+\alpha[J(u)-J(u^\dagger)]\\
&=\frac12\|Ke\|^2+\alpha\langle Kv,Ke\rangle+\alpha D_J^w(u,u^\dagger)\\
&=\frac12\|K(e+\alpha v)\|^2+\alpha D_J^w(u,u^\dagger)-\frac{\alpha^2}2\|Kv\|^2.
\end{aligned}
$$

The cross term with the residual of the [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) vanishes by the normal equation; exact data are not required. Compare the minimizing $u_\alpha$ with $z=u^\dagger-\alpha v$. At $z$, the completed square is zero. Dividing the resulting inequality by $\alpha$ proves the stronger [shifted-comparator Bregman bound](../../../../../../shifted-comparator-bregman-bound.md)

$$
\boxed{D_J^w(u_\alpha,u^\dagger)+\frac1{2\alpha}\|K(u_\alpha-u^\dagger+\alpha v)\|^2\leq D_J^w(u^\dagger-\alpha v,u^\dagger),\qquad w=K^*Kv.}
$$

Dropping the nonnegative squared term gives the requested estimate. If the comparator lies outside the effective domain of $J$, its distance is infinite and the inequality is valid but gives no finite error bound.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
