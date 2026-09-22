<h1 id="p/p2/solution">Solution</h1>

↑ **Parent:** [P2](../p2.md)

The form is symmetric and bilinear by the corresponding properties of finite real sums. Its squared [norm](../../../../norm.md) is $\langle p,p\rangle=\sum_i p(x_i)^2\geq0$. Equality means $p$ vanishes at all $n+1$ distinct nodes. A nonzero [polynomial](../../../../polynomial-split.md) of degree at most $n$ has at most $n$ roots, so equality forces $p=0$. Thus this is an [inner product](../../../../inner-product-split.md) on $\Pi_n$.

On $\Pi_{n+1}$ it is only [positive semidefinite](../../../../positive-semidefinite-matrix.md): the nonzero node [polynomial](../../../../polynomial-split.md) $\omega(x)=\prod_{i=0}^n(x-x_i)$ satisfies $\langle\omega,\omega\rangle=0$. Hence **it is not an [inner product](../../../../inner-product-split.md) on $\Pi_{n+1}$**. The [finite-evaluation inner product on polynomials](../../../../finite-evaluation-inner-product-on-polynomials.md) works exactly when the evaluation map is injective on the chosen space.

Finally, if $q\ne0$, positivity applied to $p-tq$ and the choice $t=\langle p,q\rangle/\langle q,q\rangle$ give

$$
0\leq\langle p,p\rangle-\frac{\langle p,q\rangle^2}{\langle q,q\rangle}.
$$

Rearranging proves [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) in its required form:

$$
\boxed{\left(\sum_i p(x_i)q(x_i)\right)^2\leq\left(\sum_i p(x_i)^2\right)\left(\sum_i q(x_i)^2\right)}.
$$

If $q=0$ both sides of the asserted inequality are zero. Equality holds exactly when $p,q$ are [linearly dependent](../../../../linear-dependence.md), since in the nonzero case the minimizing $p-tq$ must have zero [norm](../../../../norm.md).

## ↑ Ancestors (12)

1. [P2](../p2.md)
2. [P](../../p.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
