<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume first that $T>0$ and $-1<b<r<g$, so the [logarithmic utility](../../../../../../logarithmic-utility.md) is defined throughout the allowed [portfolio](../../../../../../investment-portfolio.md) interval. Put $A=g-r>0$ and $B=r-b>0$. Then

$$
U'(x)=-\frac{pA}{T(1+g)-Ax}+\frac{(1-p)B}{T(1+b)+Bx}.
$$

Equating this to zero and clearing the positive denominators gives

$$
x_0=T\left[\frac{(1-p)(1+g)}{g-r}-\frac{p(1+b)}{r-b}\right].
$$

The second [derivative](../../../../../../derivative.md) is strictly negative, and $U'(T)<0$ by part (c), so $x_0<T$. The [two-state logarithmic portfolio with a borrowing constraint](../../../../../../two-state-logarithmic-portfolio-with-a-borrowing-constraint.md) is therefore

$$
\boxed{x_*=\max\{0,x_0\},\qquad\text{equity investment}=T-x_*.}
$$

In particular, the threshold for all equity is

$$
p\ge p_c:=\frac{(r-b)(1+g)}{(r-b)(1+g)+(g-r)(1+b)}
=\frac{(r-b)(1+g)}{(g-b)(1+r)}.
$$

For $p<p_c$ the optimum is interior. The probability bound printed in the PDF has $1+r$ where the all-equity threshold has $1+b$. Since $1+r>1+b$, that printed lower bound is strictly below $p_c$ and does not determine which of these two cases occurs. For example, with $(b,r,g)=(0,0.1,0.3)$ its lower bound is $13/35$, while $p_c=13/33$. At $p=0.38$ all the given inequalities hold and $x_*=0.23T$; at $p=0.4$ they also hold and $x_*=0$. Thus the boxed constrained formula applies to the printed data without replacing its probability assumption.

If bad-state gross wealth can be nonpositive, the [logarithmic utility](../../../../../../logarithmic-utility.md) domain must instead be imposed explicitly. With $1+r>0$, $b\le-1$, and $0<p<1$, admissibility requires $x>-T(1+b)/(r-b)$; the same stationary root lies inside this positive-wealth interval and is optimal. If even the fully safe gross return is nonpositive, there is no admissible positive-wealth [portfolio](../../../../../../investment-portfolio.md). These domain issues are implicit in using $\log w$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
