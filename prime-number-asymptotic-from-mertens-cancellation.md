# Prime number asymptotic from Mertens cancellation

↑ **Parent:** [Mertens function](mertens-function.md)

Let $\Delta(N)=\sum_{n\le N}(\tau(n)-\log n-2\gamma)$. The [Möbius divisor-sum identity](mobius-divisor-sum-identity.md) and the [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md) give $\mu*\tau=\mathbf1$ and $\mu*\log=\Lambda$, so

$$
\psi(N)=N-2\gamma-\sum_{d\le N}\mu(d)\Delta(\lfloor N/d\rfloor).
$$

Here $*$ is [Dirichlet convolution](dirichlet-convolution.md). The [divisor summatory asymptotic](divisor-summatory-asymptotic.md) bounds the terms with $d\le N/K$ in absolute value by $O(N/\sqrt K)$. For $d>N/K$, group by $j=\lfloor N/d\rfloor<K$: the remaining sum is $\sum_{j<K}\Delta(j)(M(N/j)-M(N/(j+1)))=o_K(N)$. First let $N$ tend to infinity, then $K$ tend to infinity. This proves the [Second Chebyshev function](second-chebyshev-function.md) asymptotic from cancellation of the [Mertens function](mertens-function.md).

## ↑ Ancestors (7)

1. [Mertens function](mertens-function.md)
2. [Möbius function](mobius-function.md)
3. [Arithmetic function](arithmetic-function.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
