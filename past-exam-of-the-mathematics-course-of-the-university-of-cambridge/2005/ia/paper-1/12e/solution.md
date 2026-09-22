<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

[Rolle theorem](../../../../../rolle-theorem.md) states that if $a<b$, $f$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a)=f(b)$, then there is $c\in(a,b)$ with $f'(c)=0$.

If $f$ is constant, any interior point works. Otherwise the [extreme value theorem](../../../../../extreme-value-theorem.md) gives an attained maximum and minimum on the interval, and at least one of them differs from the common endpoint value. That extremum must occur at an interior point $c$. At an interior maximum, for small positive $h$ the difference quotient $[f(c+h)-f(c)]/h$ is nonpositive, while for negative $h$ it is nonnegative. Existence of the common derivative forces it to be both nonpositive and nonnegative, hence zero. The same argument with inequalities reversed applies to an interior minimum. This proves [Rolle theorem](../../../../../rolle-theorem.md), including the derivative-at-an-extremum step rather than assuming it.

Now let the nonconstant [polynomial](../../../../../polynomial-split.md) $p$ have distinct real roots $r_1<\cdots<r_k$, with [multiplicities](../../../../../multiplicity-mathematics.md) $m_1,\ldots,m_k$ adding to its degree $n$. If $p(x)=(x-r_j)^{m_j}q_j(x)$ and $q_j(r_j)\ne0$, differentiation gives

$$
p'(x)=(x-r_j)^{m_j-1}\bigl[m_jq_j(x)+(x-r_j)q_j'(x)\bigr].
$$

The bracket is nonzero at $r_j$, so its [multiplicity](../../../../../multiplicity-mathematics.md) as a root of $p'$ is exactly $m_j-1$. These roots already contribute $\sum_j(m_j-1)=n-k$ real roots counted with multiplicity. [Rolle theorem](../../../../../rolle-theorem.md) supplies an additional root of $p'$ in each of the $k-1$ disjoint intervals $(r_j,r_{j+1})$. These additional roots are distinct from each other and from all the $r_j$.

We have therefore exhibited at least $(n-k)+(k-1)=n-1$ real roots counted with multiplicity. The derivative has degree $n-1$, so there is no room for any additional nonreal roots. **Every root of $p'$ is real.** This is the [Rolle root count with multiplicities](../../../../../rolle-root-count-with-multiplicities.md); for $n=1$ the nonzero constant derivative has no roots, as expected.

For failure of the converse, take

$$
\boxed{p(x)=x^3+1,\qquad p'(x)=3x^2.}
$$

The derivative has only the real root zero, of multiplicity two. But $p(x)=(x+1)(x^2-x+1)$ and the quadratic factor has roots $(1\pm i\sqrt3)/2$, which are nonreal. Thus real-rootedness of the derivative does not imply real-rootedness of the original [polynomial](../../../../../polynomial-split.md).

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
