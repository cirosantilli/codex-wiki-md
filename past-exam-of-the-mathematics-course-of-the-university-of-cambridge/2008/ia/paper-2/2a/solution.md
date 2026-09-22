<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

For the [cubic population iteration](../../../../../cubic-population-iteration.md), put $g(u)=\lambda u(1-u^2)$. Its [fixed points](../../../../../fixed-point.md) solve

$$
u=g(u)\quad\Longleftrightarrow\quad u[(\lambda-1)-\lambda u^2]=0.
$$

Thus $u_*=0$ always exists. For $\lambda\ne0$ there are also

$$
\boxed{u_*=\pm\sqrt{1-\frac1\lambda}}
$$

whenever the expression under the square root is positive, namely $\lambda<0$ or $\lambda>1$. At $\lambda=1$ these coincide with zero; at $\lambda=0$ only zero exists.

The criterion for [fixed point stability for an iteration](../../../../../fixed-point-stability-for-an-iteration.md) is $|g'(u_*)|<1$. To justify it, [continuity](../../../../../continuous-function.md) of $g'$ gives a small interval around the [fixed point](../../../../../fixed-point.md) where $|g'|\leq q<1$. The [mean value theorem](../../../../../mean-value-theorem.md) then gives $|g(u)-u_*|\leq q|u-u_*|$, so this interval is invariant and the error decreases geometrically. This proves local [asymptotic stability](../../../../../asymptotic-stability.md) rather than merely linear boundedness.

Here $g'(u)=\lambda(1-3u^2)$. At zero its value is $\lambda$, so **zero is locally [asymptotically stable](../../../../../asymptotic-stability.md) for $-1<\lambda<1$**. At a nonzero [fixed point](../../../../../fixed-point.md) it is

$$
g'(u_*)=\lambda\left[1-3\left(1-\frac1\lambda\right)\right]=3-2\lambda.
$$

The strict inequality $|3-2\lambda|<1$ is equivalent to $1<\lambda<2$. Both nonzero real [fixed points](../../../../../fixed-point.md) are therefore locally [asymptotically stable](../../../../../asymptotic-stability.md) on that interval. This proves the two requested existence ranges. The strict [derivative](../../../../../derivative.md) criterion alone makes no conclusion at the endpoint multipliers of modulus one.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
