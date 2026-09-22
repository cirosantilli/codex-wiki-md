<h1 id="8a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Minkowski metric](../../../../../../minkowski-metric.md) $J=\operatorname{diag}(1,-1)$, preservation means $(Ax)^TJ(Ay)=x^TJy$ for all real [vectors](../../../../../../vector.md) $x,y$. This is equivalent to $A^TJA=J$, or, entrywise,

$$
a^2-c^2=1,\qquad b^2-d^2=-1,\qquad ab-cd=0.
$$

The restriction $a>0$ puts the first column on the right branch of the unit [hyperbola](../../../../../../hyperbola.md), so uniquely $a=\cosh t$, $c=\sinh t$ for a real parameter $t$. The third equation makes the second column a scalar multiple of $(\sinh t,\cosh t)^T$: this also covers $t=0$, when $b=0$. The second equation makes that multiple $\varepsilon=\pm1$. Thus **all the required [matrices](../../../../../../matrix.md) are**

$$
\boxed{A=H(t)D_\varepsilon=\begin{pmatrix}\cosh t&\varepsilon\sinh t\\\sinh t&\varepsilon\cosh t\end{pmatrix},\quad t\in\mathbb R,\quad\varepsilon=\pm1.}
$$

The [hyperbolic function](../../../../../../hyperbolic-function.md) addition formulas give $H(t)H(s)=H(t+s)$, while $D_\varepsilon H(s)=H(\varepsilon s)D_\varepsilon$. Consequently

$$
(H(t)D_\varepsilon)(H(s)D_\eta)=H(t+\varepsilon s)D_{\varepsilon\eta}.
$$

The product remains of the required form and its upper-left entry is positive. The identity is $H(0)D_1$, and the inverse is $H(-\varepsilon t)D_\varepsilon$. Together with associativity of [matrix multiplication](../../../../../../matrix-multiplication.md), these identities establish the [group](../../../../../../group-split.md) property. This is the [time-orientation-preserving Lorentz group in one spatial dimension](../../../../../../time-orientation-preserving-lorentz-group-in-one-spatial-dimension.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8A](../../8a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
