<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

For a [function](../../../../../function-split.md) with [continuous](../../../../../continuous-function.md) [derivatives](../../../../../derivative.md) through order $m+1$ on the interval between $0$ and $x$, the [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) is

$$
f(x)=\sum_{j=0}^{m}\frac{f^{(j)}(0)}{j!}x^j+R_m(x),\qquad
R_m(x)=\frac1{m!}\int_0^x(x-t)^m f^{(m+1)}(t)\,dt.
$$

This is [Taylor's theorem](../../../../../taylor-theorem.md) about zero; [translation](../../../../../translation-geometry.md) gives the formula about any other point. To prove it, the case $m=0$ is the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md). For $m\ge1$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
R_m(x)=-\frac{f^{(m)}(0)x^m}{m!}
+\frac1{(m-1)!}\int_0^x(x-t)^{m-1}f^{(m)}(t)\,dt
=R_{m-1}(x)-\frac{f^{(m)}(0)x^m}{m!}.
$$

Substitution into the formula at order $m-1$ proves the formula at order $m$ by induction. The [integral](../../../../../integral.md) estimate, valid also for negative $x$, is

$$
|R_m(x)|\le\frac{|x|^{m+1}}{(m+1)!}
\sup_{t\text{ between }0\text{ and }x}|f^{(m+1)}(t)|.
$$

For the [smooth function](../../../../../smooth-function.md) satisfying $f^{(3)}=f$, each fixed [derivative](../../../../../derivative.md) is [continuous](../../../../../continuous-function.md) on $[-R,R]$ and hence is bounded there by the [extreme value theorem](../../../../../extreme-value-theorem.md). Thus a bound $M_j$ exists for every $j$. Differentiating the [differential equation](../../../../../differential-equation-split.md) repeatedly gives $f^{(j+3)}=f^{(j)}$. Only the three [functions](../../../../../function-split.md) $f,f',f''$ are needed: take $M$ to be the maximum of their absolute-value bounds on $[-R,R]$. Then $|f^{(j)}(x)|\le M$ simultaneously for every $j\ge0$ and $|x|\le R$.

At zero the [derivatives](../../../../../derivative.md) consequently repeat the values $1,0,0$. [Taylor's theorem](../../../../../taylor-theorem.md) therefore gives

$$
f(x)=\sum_{n=0}^{\lfloor m/3\rfloor}\frac{x^{3n}}{(3n)!}+R_m(x),\qquad
\sup_{|x|\le R}|R_m(x)|\le\frac{MR^{m+1}}{(m+1)!}\longrightarrow0.
$$

The last [limit of a sequence](../../../../../limit-of-a-sequence.md) follows because the ratio of consecutive majorants is $R/(m+2)$, eventually less than $1/2$. Since $R$ is arbitrary, [Taylor expansion from a periodic derivative equation](../../../../../taylor-expansion-from-a-periodic-derivative-equation.md) proves

$$
\boxed{f(x)=\sum_{n=0}^{\infty}\frac{x^{3n}}{(3n)!}\quad\text{for every }x\in\mathbb R.}
$$

This proves convergence to the [function](../../../../../function-split.md) using a remainder bound; it does not assume beforehand that a [smooth function](../../../../../smooth-function.md) equals its [Taylor series](../../../../../taylor-series.md).

## ↑ Ancestors (11)

1. [12C](../12c.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
