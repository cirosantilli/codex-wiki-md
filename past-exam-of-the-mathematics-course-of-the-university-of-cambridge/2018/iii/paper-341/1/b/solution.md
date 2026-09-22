<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor the first [characteristic polynomial](../../../../../../characteristic-polynomial.md) as

$$
\rho(w)=(w-1)(w^2-2\alpha w+1).
$$

The other two [roots of a polynomial](../../../../../../root-of-a-polynomial.md) have product one. If $-1<\alpha<1$, they are $\alpha\pm i\sqrt{1-\alpha^2}$: distinct unit-modulus roots, both different from one. At $\alpha=-1$, the root $-1$ is double; at $\alpha=1$, the root one is triple. Outside $[-1,1]$, one of the reciprocal real roots has modulus greater than one. Thus the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) holds exactly for $-1<\alpha<1$.

For the [order conditions for a linear multistep method](../../../../../../order-conditions-for-a-linear-multistep-method.md), expand the exponential defect:

$$
\rho(e^z)-z\sigma(e^z)
=\frac{11-5\alpha}{6}z^3+\frac{13-7\alpha}{4}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every $\alpha$. The cubic coefficient vanishes only at $\alpha=11/5$, where the quartic coefficient is $-3/5\neq0$. Consequently the formal order is

$$
\boxed{p=\begin{cases}3,&\alpha=11/5,\\2,&\alpha\neq11/5.\end{cases}}
$$

For all parameters satisfying the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md), $\rho'(1)=\sigma(1)=2(1-\alpha)\neq0$, so this formal calculation gives ordinary second-order [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md). The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) therefore yields

$$
\boxed{\text{the method is convergent exactly when }-1<\alpha<1.}
$$

The exceptional third-order formula is not [zero-stable](../../../../../../zero-stability.md). At $\alpha=1$, $\sigma\equiv0$ and $\rho=(w-1)^3$: the recurrence contains no vector-field evaluations. It satisfies the displayed Taylor identities only formally and is **a degenerate, nonconvergent formula**, not a usable second-order ODE solver. This distinction avoids interpreting formal cancellation as convergence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
