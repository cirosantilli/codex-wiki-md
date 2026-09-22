<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) shows that the differential initial-value problem is equivalent to

$$
x(t)=x_0+\int_0^tF(s,x(s))\,ds.
$$

In one direction integrate $x'=F(t,x(t))$ from zero. In the other, continuity of the integrand makes the right side continuously differentiable with precisely that derivative and initial value.

Consider the closed subset $\mathcal X=\{x\in C([-b,b]):\|x-x_0\|_\infty\leq r\}$ of the complete space with the [uniform norm](../../../../../supremum-norm.md). It is complete: a uniformly Cauchy sequence has a uniform continuous limit, and the closed range constraint passes to the limit. Define

$$
(Tx)(t)=x_0+\int_0^tF(s,x(s))\,ds.
$$

The bound $|F|\leq C$ gives $\|Tx-x_0\|_\infty\leq bC<r$, so $T$ maps $\mathcal X$ into itself. The uniform [Lipschitz condition](../../../../../lipschitz-continuity.md) gives

$$
\boxed{\|Tx-Ty\|_\infty\leq bK\|x-y\|_\infty,\qquad q:=bK<1.}
$$

Here negative $t$ changes only the orientation of the integral; its length is still at most $b$.

Construct $x^{(0)}(t)=x_0$ and $x^{(m+1)}=Tx^{(m)}$. Induction gives $\|x^{(m+1)}-x^{(m)}\|_\infty\leq q^m\|x^{(1)}-x^{(0)}\|_\infty$. Summing this geometric bound proves uniform Cauchy convergence to some $x\in\mathcal X$. The same contraction estimate shows $Tx^{(m)}\to Tx$, so $x=Tx$. The integral equation now makes $x$ a $C^1$ solution. If another solution $y$ existed, it would also be fixed, and $\|x-y\|_\infty\leq q\|x-y\|_\infty$ would force equality. This proves **existence and uniqueness on the entire stated interval**, implementing the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) rather than just invoking it.

If $C=0$, the vector field is zero and the solution is constant. If $K=0$, the vector field is independent of the space variable and the integral solves the problem directly. The divisions by zero in the printed interval bound are naturally interpreted as imposing no restriction from the corresponding term.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
