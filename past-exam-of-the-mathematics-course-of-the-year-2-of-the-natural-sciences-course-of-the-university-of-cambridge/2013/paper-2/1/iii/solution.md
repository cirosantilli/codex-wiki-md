<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $x=\cos\theta$ and $Y(\theta)=y(\cos\theta)$, with $0\leq\theta\leq\pi$. The [chain rule](../../../../../chain-rule.md) converts $(1-x^2)y''-xy'$ to $Y''$, so $Y=\cos(n\theta)$ solves $Y''+n^2Y=0$. Hence $y_n(x)=\cos(n\arccos x)$ is a solution in the interior.

For nonnegative integer $n$, [De Moivre's theorem](../../../../../de-moivre-s-theorem.md) makes its polynomial nature explicit:

$$
\cos(n\theta)=\operatorname{Re}(\cos\theta+i\sin\theta)^n=\sum_{j=0}^{\lfloor n/2\rfloor}(-1)^j\binom n{2j}x^{n-2j}(1-x^2)^j.
$$

Every term is a polynomial of degree at most $n$. For $n\geq1$, the coefficient of $x^n$ is $\sum_j\binom n{2j}=2^{n-1}$, so its [polynomial degree](../../../../../degree-of-a-polynomial.md) is exactly $n$. These are the [Chebyshev polynomials](../../../../../chebyshev-polynomial.md) $T_n$. Their polynomial form also proves the required boundedness of the function and derivative at both endpoints. Negative labels reproduce $T_{|n|}$ and have degree $|n|$.

The first three are

$$
\boxed{y_0=1,\qquad y_1=x,\qquad y_2=2x^2-1.}
$$

Under $w\,dx=-d\theta$, their cross inner products become integrals of $1$, $\cos\theta$ and $\cos2\theta$ on $(0,\pi)$. The constant-cosine integrals vanish, and $\cos\theta\cos2\theta=(\cos\theta+\cos3\theta)/2$ also integrates to zero. Thus all three pairs are orthogonal. Their squared weighted norms are $\pi,\pi/2,\pi/2$, respectively; more generally

$$
\int_{-1}^1wT_nT_m\,dx=\begin{cases}0,&n\ne m,\\\pi,&n=m=0,\\\pi/2,&n=m\geq1.\end{cases}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
