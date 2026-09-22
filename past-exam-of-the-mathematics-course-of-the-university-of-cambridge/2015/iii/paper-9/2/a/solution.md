<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a bounded domain, the [nondivergence-form elliptic operator](../../../../../../nondivergence-form-elliptic-operator.md) obeys the [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md): $Lu\geq0$ and $c\leq0$ imply

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}=\sup_{\partial\Omega}u^+.}
$$

Here $u^+=\max\{u,0\}$. Boundedness of $\Omega$ is needed for this formulation: it is not explicitly imposed in this question. On an unbounded domain one needs an appropriate condition at infinity instead. Without either condition the claim is false, as $u(x)=x_n$ and $L=\Delta$ on the half-space $\{x_n>0\}$ show.

For the bounded-domain proof choose $\gamma>0$ so large that $\lambda\gamma^2-\|b^1\|_\infty\gamma-\|c\|_\infty>0$. The positive exponential $h(x)=e^{\gamma x_1}$ then satisfies

$$
Lh=e^{\gamma x_1}\bigl(\gamma^2a^{11}+\gamma b^1+c\bigr)>0.
$$

Let $u_\varepsilon=u+\varepsilon h$, $M=\sup_{\partial\Omega}u^+$ and $H=\sup_{\overline\Omega}h<\infty$. If $u_\varepsilon$ had a value greater than $M+\varepsilon H$, it would attain a positive maximum at an interior point. There its [gradient](../../../../../../gradient.md) vanishes and its [Hessian matrix](../../../../../../hessian-matrix.md) is [negative semidefinite](../../../../../../negative-semidefinite-matrix.md). The symmetric part of $(a^{ij})$ is [positive-definite](../../../../../../positive-definite-bilinear-form.md) by [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md), so $a^{ij}D_{ij}u_\varepsilon\leq0$; also $cu_\varepsilon\leq0$. Hence $Lu_\varepsilon\leq0$, contradicting $Lu_\varepsilon=Lu+\varepsilon Lh>0$. Thus $u_\varepsilon\leq M+\varepsilon H$. Letting $\varepsilon\downarrow0$ proves the [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md), without requiring continuity of the coefficients.

For example, the unbounded-domain version follows by exhausting the domain with bounded truncations if $\limsup_{|x|\to\infty,\,x\in\Omega}u(x)\leq M$: the added spherical boundaries then have supremum at most $M+o(1)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
