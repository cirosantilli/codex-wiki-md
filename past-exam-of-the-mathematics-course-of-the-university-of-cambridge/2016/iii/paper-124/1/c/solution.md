<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $M(x)=\sum_{n\le x}\mu(n)$ be the [Mertens function](../../../../../../mertens-function.md). [Partial summation](../../../../../../abel-s-summation-formula.md) gives

$$
\sum_{n\le X}\frac{\mu(n)}{n^s}=M(X)X^{-s}+s\int_1^X M(x)x^{-s-1}\,dx.
$$

For any $\Re s>0.9$, choose a sufficiently small $\epsilon>0$ with $0.9+\epsilon<\Re s$. The assumed bound makes the boundary term tend to zero and makes the integral absolutely convergent. Moreover, on each [compact set](../../../../../../compact-space.md) of this half-plane, one can choose the same $\epsilon$, so the integral has [locally uniform convergence](../../../../../../locally-uniform-convergence.md). Hence

$$
F(s)=s\int_1^\infty M(x)x^{-s-1}\,dx
$$

is a [holomorphic function](../../../../../../holomorphic-function.md) on $\Re s>0.9$, agreeing with the reciprocal [Dirichlet series](../../../../../../dirichlet-series.md) from part (b) on $\Re s>1$.

The [identity theorem](../../../../../../identity-theorem.md) applied to the [holomorphic functions](../../../../../../holomorphic-function.md) $(s-1)\zeta(s)F(s)$ and $s-1$ extends their equality throughout $\Re s>0.9$; the assumed simple [pole](../../../../../../pole.md) makes the first function holomorphic at $1$. Thus $\zeta(s)F(s)=1$ away from $1$, proving **a zero-free half-plane**:

$$
\boxed{\zeta(s)\ne0\quad\text{if }\Re s>0.9,\ s\ne1.}
$$

To obtain the strongest symmetric conclusion, use the following basic facts explicitly: the [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md) gives the [entire function](../../../../../../entire-function.md) $\xi(s)=\tfrac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)$ with $\xi(s)=\xi(1-s)$, and the [trivial zeros of the Riemann zeta function](../../../../../../trivial-zero-of-the-riemann-zeta-function.md) are the negative even integers. Every [Nontrivial zero of the Riemann zeta function](../../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) is therefore accompanied by its reflection $1-s$. A [Nontrivial zero of the Riemann zeta function](../../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) with real part below $0.1$ would reflect to one above $0.9$, which is impossible. Consequently **all nontrivial zeros lie in the closed strip**

$$
\boxed{0.1\le\Re\rho\le0.9.}
$$

The $\epsilon$ in the hypothesis prevents this argument from excluding either boundary line; the [trivial zeros of the Riemann zeta function](../../../../../../trivial-zero-of-the-riemann-zeta-function.md) remain present.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
