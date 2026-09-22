<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [Taylor formula with integral remainder](../../../../../taylor-formula-with-integral-remainder.md) is

$$
\boxed{f(x)=\sum_{j=0}^n\frac{f^{(j)}(a)}{j!}(x-a)^j+R_n(f,a,x),\qquad
R_n(f,a,x)=\frac1{n!}\int_a^x(x-t)^n f^{(n+1)}(t)\,dt.}
$$

For $n=0$, this is the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md). [Integration by parts](../../../../../integration-by-parts.md) gives

$$
R_n(f,a,x)=-\frac{f^{(n)}(a)}{n!}(x-a)^n+R_{n-1}(f,a,x).
$$

Rearranging and applying [mathematical induction](../../../../../mathematical-induction.md) proves the displayed expansion. The oriented integral also covers $x<a$.

For $x\ne0$, the [chain rule](../../../../../chain-rule.md) and [product rule](../../../../../product-rule.md) give

$$
f'(x)=\left[2x^{-3}p(1/x)-x^{-2}p'(1/x)\right]e^{-1/x^2}.
$$

Thus

$$
\boxed{q(t)=2t^3p(t)-t^2p'(t).}
$$

Because [Gaussian decay dominates every power](../../../../../gaussian-decay-dominates-every-power.md), $p(1/x)e^{-1/x^2}/x\to0$ as $x\to0$. Hence $f'(0)=0$, and the derivative formula extends continuously to zero. Repeating the argument replaces $p$ by another polynomial at each step: $p_{j+1}(t)=2t^3p_j(t)-t^2p_j'(t)$. All derivative difference quotients at zero tend to zero, so the [polynomial multiples of a Gaussian flat function](../../../../../polynomial-multiples-of-a-gaussian-flat-function.md) are [smooth functions](../../../../../smooth-function.md) with

$$
f^{(j)}(0)=0\qquad(j\ge0).
$$

The [Taylor polynomial](../../../../../taylor-polynomial.md) about zero is therefore identically zero for every degree, and

$$
\boxed{R_n(f,0,x)=f(x)\quad\text{for every }n.}
$$

A nonzero polynomial has only finitely many [roots of a polynomial](../../../../../root-of-a-polynomial.md), so $p(1/x)\ne0$ for every sufficiently small nonzero $x$. At each such fixed $x$, this remainder never tends to zero. The [flat function](../../../../../flat-function.md) is therefore smooth but not [real analytic](../../../../../real-analytic-function.md) at zero.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
