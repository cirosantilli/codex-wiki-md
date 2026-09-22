<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For real continuous $f$, the [Chebyshev alternation theorem](../../../../../equioscillation-theorem.md) says that $p\in\mathcal P_n$ is the unique [best uniform approximation](../../../../../best-uniform-approximation.md) to $f$ precisely when there are $n+2$ ordered points $0\le x_0<\cdots<x_{n+1}\le1$ and a sign $\sigma\in\{-1,1\}$ such that

$$
f(x_j)-p(x_j)=\sigma(-1)^j\|f-p\|_\infty.
$$

Here $\mathcal P_n$ means degree at most $n$. Best approximants exist: a minimizing sequence is bounded in the finite-dimensional [polynomial](../../../../../polynomial-split.md) space, and [finite-dimensional equivalence of norms](../../../../../finite-dimensional-equivalence-of-norms.md) gives a convergent [coefficient](../../../../../coefficient.md) subsequence. When $f=p$, the zero error is treated separately; the derivative-sign hypothesis below excludes that case.

Let $p_n$ be a best degree-at-most-$n$ approximant and suppose for contradiction that $E_n(f)=E_{n+1}(f)$. Since $f^{(n+1)}>0$, $f$ is not a degree-at-most-$n$ [polynomial](../../../../../polynomial-split.md) and its error is nonzero. The same $p_n$ would be best in $\mathcal P_{n+1}$, so the [Chebyshev alternation theorem](../../../../../equioscillation-theorem.md) at that degree supplies $n+3$ alternating error extrema. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives at least $n+2$ distinct zeros of $e=f-p_n$, one between each consecutive pair of extrema.

Repeated [Rolle's theorem](../../../../../rolle-theorem.md) then forces a zero of $e^{(n+1)}$. But $p_n^{(n+1)}=0$, whereas $e^{(n+1)}=f^{(n+1)}>0$ everywhere. This contradiction proves

$$
\boxed{E_n(f)>E_{n+1}(f).}
$$

The argument proves [strict decrease of best polynomial approximation under a derivative sign](../../../../../strict-decrease-of-best-polynomial-approximation-under-a-derivative-sign.md); an everywhere negative $(n+1)$st [derivative](../../../../../derivative.md) gives the same strict conclusion after replacing $f$ by $-f$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
