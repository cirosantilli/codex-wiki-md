<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [backward option pricing](../../../../../../backward-option-pricing.md) recursion is

$$
V(n-1,s)
=\frac{qV(n,s(1+b))+(1-q)V(n,s(1+a))}{1+r},
$$

with terminal value $V(N,s)=g(s)$. At a node with $S_{n-1}=s$, define the [replicating](../../../../../../replicating-portfolio-in-a-binomial-market.md) stock holding by

$$
\boxed{
\theta_n
=\frac{V(n,s(1+b))-V(n,s(1+a))}
{s(b-a)}}.
$$

This is a [predictable process](../../../../../../predictable-process.md) because it depends only on information available at time $n-1$.

Indeed, if $X_{n-1}=V(n-1,s)$, substituting the risk-neutral formula for $q$ into the self-financing update shows separately in the up and down states that

$$
X_n=V(n,S_n).
$$

An induction over $n$ therefore gives $X_N=V(N,S_N)=g(S_N)$. The required initial capital is

$$
\boxed{x=V(0,S_0)=(1+r)^{-N}\mathbb E_Q[g(S_N)]}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
