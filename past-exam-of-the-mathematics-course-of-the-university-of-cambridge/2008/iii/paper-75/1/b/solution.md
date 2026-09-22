<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The exponents are real, as required for this family of real [continuous functions](../../../../../../continuous-function.md). We prove the [exponential Chebyshev system](../../../../../../exponential-chebyshev-system.md) property by induction on the number of [functions](../../../../../../function-split.md). A single nonzero multiple of an [exponential function](../../../../../../exponential-function.md) has no zero, so the base case holds.

Suppose the result holds for $n$ distinct real exponents, and consider a nontrivial combination $F(x)=\sum_{j=0}^n c_je^{\lambda_jx}$. If it had $n+1$ distinct zeros, so would

$$
g(x)=e^{-\lambda_0x}F(x)=c_0+\sum_{j=1}^n c_je^{(\lambda_j-\lambda_0)x},
$$

since the prefactor is everywhere positive. Applying [Rolle's theorem](../../../../../../rolle-theorem.md) between consecutive zeros gives at least $n$ distinct zeros of

$$
g'(x)=\sum_{j=1}^n c_j(\lambda_j-\lambda_0)e^{(\lambda_j-\lambda_0)x}.
$$

The $n$ exponents in this [derivative](../../../../../../derivative.md) are distinct. By induction, a nontrivial combination of them has at most $n-1$ zeros. Therefore every coefficient $c_j(\lambda_j-\lambda_0)$ must be zero. Distinctness gives $c_j=0$ for $j\ge1$. Then $g=c_0$ has a zero only if $c_0=0$, contradicting the original nontriviality. Consequently $F$ has at most $n$ zeros, and

$$
\boxed{(e^{\lambda_0x},\ldots,e^{\lambda_nx})\text{ is a Chebyshev system on }[a,b].}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
