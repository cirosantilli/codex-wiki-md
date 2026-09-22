<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

For real functions $u,v$ that are continuously differentiable on a closed interval $[a,b]$, [integration by parts](../../../../../integration-by-parts.md) states

$$
\boxed{\int_a^b u(x)v'(x)\,dx=[u(x)v(x)]_a^b-\int_a^b u'(x)v(x)\,dx.}
$$

It follows from the [product rule](../../../../../product-rule.md) and the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md). With the convention $\int_a^b=-\int_b^a$, the identity also applies to reversed limits. These regularity assumptions ensure that all the proper integrals exist.

For the smooth $f$ in the problem, define the [integral remainder in Taylor theorem](../../../../../integral-remainder-in-taylor-theorem.md) by

$$
R_n(t)=\frac1{(n-1)!}\int_0^t f^{(n)}(x)(t-x)^{n-1}\,dx.
$$

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives $f(t)=f(0)+R_1(t)$. Applying [integration by parts](../../../../../integration-by-parts.md) to $R_n$, with $u=f^{(n)}(x)$ and antiderivative $v=-(t-x)^n/n!$ of $(t-x)^{n-1}/(n-1)!$, gives

$$
R_n(t)=\frac{f^{(n)}(0)t^n}{n!}+\frac1{n!}\int_0^t f^{(n+1)}(x)(t-x)^n\,dx=\frac{f^{(n)}(0)t^n}{n!}+R_{n+1}(t).
$$

Induction starting from $n=1$ therefore proves

$$
\boxed{f(t)=\sum_{k=0}^{n-1}\frac{f^{(k)}(0)t^k}{k!}+\frac1{(n-1)!}\int_0^t f^{(n)}(x)(t-x)^{n-1}\,dx.}
$$

The same calculation holds for negative $t$: all integrals are oriented, and the segment joining $0$ and $t$ lies in $(-1,1)$. Thus the proof covers every stated $t$ and every positive integer $n$.

Now take $f(x)=\log(1-x)$. For $k\ge1$, differentiation gives $f^{(k)}(x)=-(k-1)!/(1-x)^k$, and $f(0)=0$. With $n=N+1$ and $t=1/2$, the [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) becomes

$$
\log2=\sum_{k=1}^N\frac1{k2^k}+J_N,\qquad J_N=\int_0^{1/2}\frac{(1/2-x)^N}{(1-x)^{N+1}}\,dx.
$$

For $0\le x\le1/2$, $0\le(1/2-x)/(1-x)\le1/2$ and $(1-x)^{-1}\le2$. Hence $0\le J_N\le2^{-N}$ after integrating over an interval of length $1/2$. Thus the [logarithmic series from an integral Taylor remainder](../../../../../logarithmic-series-from-an-integral-taylor-remainder.md) satisfies

$$
\boxed{\sum_{k=1}^\infty\frac1{k2^k}=\log2,\qquad 0\le\log2-\sum_{k=1}^N\frac1{k2^k}\le2^{-N}.}
$$

The explicit vanishing remainder establishes convergence and identifies the sum, without using a pre-existing logarithmic power series.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
