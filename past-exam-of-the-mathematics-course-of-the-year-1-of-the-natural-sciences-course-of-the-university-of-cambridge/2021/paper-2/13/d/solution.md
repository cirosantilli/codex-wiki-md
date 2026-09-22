<h1 id="13/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The original PDF has angle $\theta(t)=2\pi t^n$, with $n$ an exponent on $t$. It is not $2\pi nt$: each permitted value of $n$ changes the speed but traverses the same circle once counterclockwise. Along the path, $r^2=2$ and

$$
\boldsymbol r'(t)=\theta'(t)(-\sin\theta,\cos\theta,0),\qquad
\theta'=2\pi n t^{n-1}.
$$

The radial contribution to the [line integral](../../../../../line-integral.md) vanishes, since $(\cos\theta,\sin\theta,1)\cdot(-\sin\theta,\cos\theta,0)=0$. The rotational contribution gives

$$
\boldsymbol F(\boldsymbol r(t))\cdot\boldsymbol r'(t)=a\theta'(t).
$$

Therefore

$$
\boxed{\int_\Gamma\boldsymbol F\cdot d\boldsymbol r
=a[\theta(1)-\theta(0)]=2\pi a,\qquad n=1,2,\ldots.}
$$

The answer is independent of the monotone parametrization, as an oriented [line integral](../../../../../line-integral.md) should be.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [13](../../13.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
