<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The product $(\tanh s)y(s)$ is continuous, so the [fundamental theorem of calculus](../../../fundamental-theorem-of-calculus.md) makes the integral continuously differentiable. Differentiating the integral equation and then evaluating at zero gives $y'=(\tanh x)y$, $y(0)=1$. Since $(\log\cosh x)'=\tanh x$, an [integrating factor](../../../integrating-factor.md) is $1/\cosh x$. Thus $(y/\cosh x)'=0$, and

$$
\boxed{y(x)=\cosh x.}
$$

Put $L(x)=\log\cosh x$, so $L(0)=0$ and $L'=\tanh x$. The claimed [Picard iterate](../../../picard-iterate.md) formula holds for $n=0$. Assuming it at $n$, termwise integration of the finite sum gives

$$
y_{n+1}(x)=1+\sum_{k=0}^n\frac1{k!}\int_0^xL(s)^kL'(s)ds
=1+\sum_{k=0}^n\frac{L(x)^{k+1}}{(k+1)!}.
$$

This proves by induction

$$
\boxed{y_n(x)=\sum_{k=0}^n\frac{(\log\cosh x)^k}{k!}\longrightarrow e^{\log\cosh x}=\cosh x.}
$$

The same calculation works for negative $x$ because it uses an antiderivative rather than a monotonicity substitution. On every bounded interval $|x|\leq R$, $0\leq L(x)\leq\log\cosh R$, so comparison with the exponential-series tail also proves uniform convergence there.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2010](../../2010-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
