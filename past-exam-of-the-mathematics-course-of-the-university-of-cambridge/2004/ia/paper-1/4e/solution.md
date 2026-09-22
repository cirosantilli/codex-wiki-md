<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

For the first [derivative](../../../../../derivative.md), $f'(x)=\tfrac12(1+x)^{-1/2}$, which is the stated formula at $r=1$. If the formula holds at $r$, differentiating multiplies its coefficient by $\tfrac12-r=-(2r-1)/2$. The factorial coefficients satisfy

$$
\frac{(2r-2)!}{2^{2r-1}(r-1)!}\frac{2r-1}{2}
=\frac{(2r)!}{2^{2r+1}r!}.
$$

The sign changes, proving by [mathematical induction](../../../../../mathematical-induction.md) that

$$
\boxed{f^{(r)}(x)=(-1)^{r-1}\frac{(2r-2)!}{2^{2r-1}(r-1)!}
(1+x)^{1/2-r}\qquad(r\geq1).}
$$

Apply the given [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) at $x=1/2$. Its polynomial part is $1+2S_n$, where $S_n$ is the first $n$ terms of the requested series, since

$$
\frac{f^{(r)}(0)}{r!}2^{-r}
=2(-1)^{r-1}\frac{(2r-2)!}{8^r r!(r-1)!}.
$$

To justify passage to the infinite [series](../../../../../series-mathematics.md), for $0\leq t\leq1/2$,

$$
|f^{(n+1)}(t)|\leq\frac{(2n)!}{2^{2n+1}n!}.
$$

Therefore the integral remainder obeys

$$
\begin{aligned}
|R_n(1/2)|
&\leq\frac{(2n)!}{2^{2n+1}(n!)^2}
\frac{2^{-(n+1)}}{n+1}\\
&=\frac{\binom{2n}{n}}{2^{3n+2}(n+1)}
\leq\frac{2^{-n-2}}{n+1}\longrightarrow0.
\end{aligned}
$$

The last inequality follows from $\binom{2n}{n}\leq\sum_{j=0}^{2n}\binom{2n}{j}=4^n$, a direct [binomial theorem](../../../../../binomial-theorem.md) bound. Hence $\sqrt{3/2}=1+2\lim S_n$, and

$$
\boxed{\sum_{r=1}^{\infty}(-1)^{r-1}\frac{(2r-2)!}{8^r r!(r-1)!}
=\frac{\sqrt6-2}{4}.}
$$

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
