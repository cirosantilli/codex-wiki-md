<h1 id="2f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $p_*(x)=2^{1-n}T_n(x)$, a monic [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md). Its norm on $[-1,1]$ is $2^{1-n}$. At the ordered points $x_j=\cos((n-j)\pi/n)$, its values alternate between the two extreme values $\pm2^{1-n}$.

Approximate $f(x)=x^n$ by [polynomials](../../../../../../polynomial-split.md) of degree at most $n-1$. The error corresponding to $q_*=x^n-p_*$ is exactly $p_*$. The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) therefore makes $q_*$ the unique best approximant. For any monic $p$, the [polynomial](../../../../../../polynomial-split.md) $q=x^n-p$ is an admissible approximant, so

$$
\boxed{\|p\|_\infty=\|x^n-q\|_\infty\geq\|p_*\|_\infty=2^{1-n}.}
$$

Equality holds precisely for $p=p_*$. Alternatively, a smaller norm would force $p-p_*$ to change sign between each consecutive pair of alternating extrema, giving at least $n$ zeros to a [polynomial](../../../../../../polynomial-split.md) of degree at most $n-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2F](../../2f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
