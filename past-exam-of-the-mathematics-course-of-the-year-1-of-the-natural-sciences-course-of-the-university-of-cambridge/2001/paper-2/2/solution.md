<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [generalized Leibniz rule](../../../../generalized-leibniz-rule.md) follows by [mathematical induction](../../../../mathematical-induction.md). The case $n=0$ is the identity $uv=uv$. Suppose the formula holds for $n$ and differentiate every term using the [product rule](../../../../product-rule.md):

$$
(uv)^{(n+1)}=\sum_{r=0}^n\binom nr\left[u^{(r+1)}v^{(n-r)}+u^{(r)}v^{(n-r+1)}\right].
$$

For an interior index $r$, the coefficient of $u^{(r)}v^{(n+1-r)}$ becomes $\binom n{r-1}+\binom nr=\binom{n+1}r$ by [Pascal's identity](../../../../pascal-s-rule.md). The two endpoint coefficients are one. This proves

$$
\boxed{(uv)^{(n)}=\sum_{r=0}^n\binom nr u^{(r)}v^{(n-r)},\qquad\binom nr=\frac{n!}{r!(n-r)!}.}
$$

Only finitely many [derivatives](../../../../derivative.md) are involved; it suffices that both [functions](../../../../function-split.md) are $n$ times differentiable.

For $u=x(x+1)$ and $v=e^{2x}$, the [derivatives](../../../../derivative.md) of $u$ beyond order two vanish. The three surviving terms of the [generalized Leibniz rule](../../../../generalized-leibniz-rule.md) give

$$
\begin{aligned}
\frac{d^n}{dx^n}\bigl[x(x+1)e^{2x}\bigr]
&=e^{2x}\left[2^n(x^2+x)+n2^{n-1}(2x+1)+n(n-1)2^{n-2}\right]\\
&=\boxed{2^ne^{2x}\left[x^2+(n+1)x+\frac{n(n+1)}4\right].}
\end{aligned}
$$

The simplified expression works for every integer $n\geq0$, including the two cases where one or more of the three terms are absent.

For $u=x^2$ and $v=\sin x$, use $d^m(\sin x)/dx^m=\sin(x+m\pi/2)$. Again only three terms survive. With $T=x+n\pi/2$, they are

$$
\frac{d^n}{dx^n}(x^2\sin x)=x^2\sin T+2nx\sin(T-\pi/2)+n(n-1)\sin(T-\pi).
$$

Since $\sin(T-\pi/2)=-\cos T$ and $\sin(T-\pi)=-\sin T$, this becomes

$$
\boxed{\frac{d^n}{dx^n}(x^2\sin x)=\bigl[x^2-n(n-1)\bigr]\sin\left(x+\frac{n\pi}2\right)-2nx\cos\left(x+\frac{n\pi}2\right).}
$$

The factors $n$ and $n(n-1)$ remove the nonexistent terms when $n=0$ or $1$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
