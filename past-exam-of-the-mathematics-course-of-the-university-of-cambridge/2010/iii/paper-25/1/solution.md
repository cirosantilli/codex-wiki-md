<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\mathbf1(n)=1$ and let $\varepsilon$ be the [identity for Dirichlet convolution](../../../../../identity-for-dirichlet-convolution.md). The [Möbius function](../../../../../mobius-function.md) uses the empty-product convention $\mu(1)=1$; the [Von Mangoldt function](../../../../../von-mangoldt-function.md) has $\Lambda(1)=0$. We first establish all the [arithmetic function](../../../../../arithmetic-function.md) identities needed below. Every [integer divisor](../../../../../divisor.md) of $n$ contributes one to $\tau(n)$, so $\tau=\mathbf1*\mathbf1$. If $n>1$ has $r$ distinct [prime factors](../../../../../prime-factor.md), the squarefree divisors correspond to their subsets and

$$
\sum_{d\mid n}\mu(d)=\sum_{j=0}^r\binom rj(-1)^j=(1-1)^r=0.
$$

At $n=1$ the sum is one. Thus $\mu*\mathbf1=\varepsilon$. Writing $n=\prod_p p^{v_p(n)}$, the only divisors with nonzero [Von Mangoldt function](../../../../../von-mangoldt-function.md) are $p,p^2,\ldots,p^{v_p(n)}$, and hence

$$
\sum_{d\mid n}\Lambda(d)=\sum_p v_p(n)\log p=\log n.
$$

The [Dirichlet convolution](../../../../../dirichlet-convolution.md) is commutative by replacing $d$ with $n/d$, and associative because either bracketing sums $f(a)g(b)h(c)$ over $abc=n$. Consequently

$$
\boxed{\mu*\tau=\mathbf1,\qquad\mu*\log=\Lambda.}
$$

These are consequences of the definitions, rather than unproved invocations of [Möbius inversion](../../../../../mobius-inversion-formula.md).

To identify the constant, integrate on each interval $[j,j+1)$:

$$
\int_j^{j+1}\frac{\{x\}}{x\lfloor x\rfloor}\,dx
=\frac1j-\log\frac{j+1}{j}.
$$

The tail is $O(1/J)$, since the integrand is at most $2/x^2$ for $x\ge2$. Summation therefore gives $\gamma=\lim_{J\to\infty}(H_J-\log(J+1))$, where $H_J$ is the [harmonic number](../../../../../harmonic-number.md), and $H_J=\log J+\gamma+O(1/J)$. Thus this is [Euler's constant](../../../../../euler-s-constant.md).

Put $r=\lfloor\sqrt N\rfloor$. Counting pairs of [positive integers](../../../../../positive-integer.md) whose product is at most $N$, and subtracting the square counted twice, gives the [Dirichlet hyperbola method](../../../../../dirichlet-hyperbola-method.md) identity

$$
D(N):=\sum_{n\le N}\tau(n)
=2\sum_{a\le r}\left\lfloor\frac Na\right\rfloor-r^2
=2NH_r-r^2+O(r).
$$

Since $r=\sqrt N+O(1)$, the [harmonic number](../../../../../harmonic-number.md) estimate yields

$$
D(N)=N\log N+(2\gamma-1)N+O(\sqrt N).
$$

The increasing [natural logarithm](../../../../../natural-logarithm.md) also satisfies $\sum_{n\le N}\log n=N\log N-N+O(\log(2N))$ by comparison with its integral. Subtracting proves

$$
\boxed{\Delta(N)=O(\sqrt N).}
$$

For the second implication, denote the [Mertens function](../../../../../mertens-function.md) by $M(x)$ and the [Second Chebyshev function](../../../../../second-chebyshev-function.md) by $\psi(x)$. Apply the proved [Dirichlet convolution](../../../../../dirichlet-convolution.md) identities to $b(n)=\tau(n)-\log n-2\gamma\mathbf1(n)$:

$$
\mu*b=\mathbf1-\Lambda-2\gamma\varepsilon.
$$

Summing this identity over integers up to $N$ gives the exact relation

$$
\psi(N)=N-2\gamma-E(N),\qquad
E(N)=\sum_{d\le N}\mu(d)\Delta(\lfloor N/d\rfloor).
$$

Fix an integer $K\ge2$. The contribution to $E(N)$ from $d\le N/K$ has absolute value at most

$$
C\sqrt N\sum_{d\le N/K}d^{-1/2}\ll\frac N{\sqrt K}.
$$

For $d>N/K$, group by $j=\lfloor N/d\rfloor$. This gives exactly

$$
\sum_{j=1}^{K-1}\Delta(j)
\left(M(N/j)-M(N/(j+1))\right)=o_K(N)
$$

under the assumed cancellation $M(x)=o(x)$; extending that assumption from integers to real $x$ uses $M(x)=M(\lfloor x\rfloor)$. Therefore $\limsup_{N\to\infty}|E(N)|/N\ll K^{-1/2}$. Letting $K\to\infty$ proves the [prime number asymptotic from Mertens cancellation](../../../../../prime-number-asymptotic-from-mertens-cancellation.md):

$$
\boxed{\frac{\psi(N)}N=1+o(1).}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
