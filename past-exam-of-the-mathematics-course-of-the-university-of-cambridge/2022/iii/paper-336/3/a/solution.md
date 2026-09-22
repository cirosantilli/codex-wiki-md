<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The reduced outer equation is $(1+x)y_0'+y_0=0$. Imposing the right boundary condition gives

$$
\boxed{y_{\rm out}=\frac2{1+x}
+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]+O(\epsilon^2).}
$$

The condition at $x=0$ requires $X=x/\epsilon$. The first two inner terms are

$$
\boxed{Y_0=2-e^{-X},
\qquad
Y_1=-2X+\frac32+\left(\frac{X^2}{2}-\frac32\right)e^{-X}.}
$$

They match $2+\epsilon(-2X+3/2)$. The [additive composite expansion](../../../../../../additive-composite-expansion.md) is

$$
\boxed{
y_{\rm comp}=\frac2{1+x}
+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]
-e^{-x/\epsilon}
+\epsilon\left[\frac12\left(\frac x\epsilon\right)^2-\frac32\right]e^{-x/\epsilon}.}
$$

On $[-1,1]$, the coefficient $1+x$ vanishes at the left endpoint. The ordinary $O(\epsilon)$ exponential layer is replaced by a turning-point endpoint region of width $O(\sqrt\epsilon)$, where all three terms in the equation enter the leading balance.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
