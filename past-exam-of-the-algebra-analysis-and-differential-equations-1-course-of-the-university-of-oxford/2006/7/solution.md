<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [fundamental theorem of calculus](../../../fundamental-theorem-of-calculus.md) first gives $y'(x)=1+\int_0^x f(y(s))\,ds$. Integrating again, or differentiating the proposed expression twice and checking its initial values, yields the [Volterra integral equation](../../../volterra-integral-equation.md)

$$
\boxed{y(x)=x+\int_0^x(x-s)f(y(s))\,ds.}
$$

For $f(y)=-y$, the [initial value problem](../../../initial-value-problem.md) is solved by $\boxed{y(x)=\sin x}$. Its [Picard iteration](../../../picard-iteration.md) constructs the sine series directly. The base approximation is $y_0(x)=x$. If

$$
y_n(x)=\sum_{k=0}^n(-1)^k\frac{x^{2k+1}}{(2k+1)!},
$$

then elementary integration gives

$$
\int_0^x(x-s)\frac{s^{2k+1}}{(2k+1)!}\,ds=\frac{x^{2k+3}}{(2k+3)!}.
$$

Substituting this finite sum in the next update, then shifting its index, proves the same formula with $n+1$ in place of $n$. This is the required [mathematical induction](../../../mathematical-induction.md). The resulting partial sums converge to $\boxed{\sin x}$ for every real $x$, and uniformly on every bounded interval: the absolute terms on $|x|\le R$ are bounded by the convergent series $\sum_kR^{2k+1}/(2k+1)!$.

The printed update lists $n=1,2,\ldots$, which would leave $y_1$ unspecified if read literally. The usual [Picard iteration](../../../picard-iteration.md), and the requested induction from $y_0$, use the update starting at $n=0$; that intended convention is used here.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2006](../../2006-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
