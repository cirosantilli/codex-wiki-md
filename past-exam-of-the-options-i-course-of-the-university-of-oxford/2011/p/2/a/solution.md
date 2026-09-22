<h1 id="p/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $x=\cos\theta$ with $0\leq\theta\leq\pi$. The cosine addition identity gives

$$
\cos((n+1)\theta)+\cos((n-1)\theta)=2\cos\theta\cos(n\theta),
$$

hence $T_0=1$, $T_1=x$, and $T_{n+1}=2xT_n-T_{n-1}$. By [mathematical induction](../../../../../mathematical-induction.md), $T_n$ is a [polynomial](../../../../../polynomial-split.md) of degree $n$: the initial cases hold, and the leading term of $2xT_n$ has degree $n+1$ while the subtraction has lower degree. Its leading coefficient is $2^{n-1}$ for $n\geq1$.

The same change of variables gives the weighted [integral](../../../../../integral-split.md)

$$
\int_{-1}^1\frac{T_n(x)}{\sqrt{1-x^2}}\,dx=\int_0^\pi\cos(n\theta)\,d\theta
=\boxed{\begin{cases}\pi,&n=0,\\0,&n\geq1.\end{cases}}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
