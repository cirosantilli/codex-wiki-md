<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Retaining the nonlinear factor $f$ determines the order-$\epsilon$ forcing and the matching constants. Write $\delta=\sqrt\epsilon$. The inner leading equation and its [boundary condition](../../../../../boundary-condition.md) at $r=1$ give $f_0=C(1-r^{-1/2})$. Matching to the far-field value fixes $C=1$.

The tail $-r^{-1/2}$ becomes $-\delta x^{-1/2}$ under $x=\epsilon r$, so a regular expansion in integer powers of $\epsilon$ cannot suffice. This is a [matched expansion with square-root and logarithmic corrections](../../../../../matched-expansion-with-square-root-and-logarithmic-corrections.md). Define

$$
E(x)=\int_x^\infty t^{-3/2}e^{-t}\,dt,
\qquad E'=-x^{-3/2}e^{-x},
\qquad E=2x^{-1/2}-2\sqrt\pi+2\sqrt x+O(x^{3/2}).
$$

The [exponential integral](../../../../../exponential-integral.md) here is normalized by the displayed definite integral. [Integration by parts](../../../../../integration-by-parts.md) also gives $E(x)=2e^{-x}/\sqrt x-2\sqrt\pi\operatorname{erfc}\sqrt x$, using the [complementary error function](../../../../../complementary-error-function.md).

For the outer [asymptotic expansion](../../../../../asymptotic-expansion.md), put $F(x)=f(x/\epsilon)$ and

$$
F=1+\delta F_1+\delta^2F_2+\cdots,\qquad
L g=g''+\left(\frac{3}{2x}+1\right)g'.
$$

The transformed equation gives $LF_1=0$ and $LF_2=-F_1F_1'$, with both corrections vanishing at infinity. Matching the leading inner tail determines $F_1=-E/2$. Multiplying the equation for $F_2$ by its [integrating factor](../../../../../integrating-factor.md) yields

$$
\left(x^{3/2}e^xF_2'\right)'=\frac14 E(x).
$$

Fix the particular solution $G$ unambiguously by

$$
I(x)=\int_0^x E(s)\,ds
=\sqrt\pi\operatorname{erf}\sqrt x+xE(x),\qquad
G(x)=-\int_x^\infty t^{-3/2}e^{-t}I(t)\,dt.
$$

Then $(x^{3/2}e^xG')'=E$, $G(\infty)=0$, and $G$ has no $x^{-1/2}$ term at zero. The general outer correction is $F_2=\beta E+G/4$, where

$$
G(x)=4\log x+\mu+O(\sqrt x).
$$

The logarithm in this [asymptotic expansion](../../../../../asymptotic-expansion.md) explains why the inner expansion needs an $\epsilon\log\epsilon$ term.

For the inner [asymptotic expansion](../../../../../asymptotic-expansion.md), all corrections larger than order $\epsilon$ solve the homogeneous leading equation and vanish at $r=1$. At order $\epsilon$, the forcing is

$$
f_2''+\frac{3}{2r}f_2'=-f_0f_0'
=-\frac12r^{-3/2}+\frac12r^{-2}.
$$

Integration gives the particular solution $1-\sqrt r+\log r$, which vanishes at $r=1$. Thus write

$$
f=(1+\delta A+\epsilon C\log\epsilon+\epsilon B)(1-r^{-1/2})
+\epsilon(1-\sqrt r+\log r)+o(\epsilon).
$$

Express this inner expansion in $x=\epsilon r$ and compare the terms that survive in the overlap $\epsilon\ll x\ll1$. The order-$\delta$ constant gives $A=\sqrt\pi$. At order $\epsilon$, the term $C\log\epsilon+\log r$ becomes $\log x+(C-1)\log\epsilon$, so $C=1$. The singular term $-\epsilon A/\sqrt x$ matches $2\epsilon\beta/\sqrt x$, giving $\beta=-\sqrt\pi/2$. Finally, the regular constants give $B+1=\pi+\mu/4$.

The requested expansions, including every correction through order $\epsilon$, are therefore

$$
\boxed{\begin{aligned}
f(r,\epsilon)={}&\left[1+\sqrt{\pi\epsilon}+\epsilon\log\epsilon
+\epsilon\left(\pi+\frac\mu4-1\right)\right](1-r^{-1/2})\\
&+\epsilon(1-\sqrt r+\log r)+o(\epsilon),\qquad r\ \text{fixed},\\
f(x/\epsilon,\epsilon)={}&1-\frac{\sqrt\epsilon}{2}E(x)
+\epsilon\left[-\frac{\sqrt\pi}{2}E(x)+\frac14G(x)\right]
+o(\epsilon),\qquad x>0\ \text{fixed}.
\end{aligned}}
$$

The inner formula satisfies the [boundary condition](../../../../../boundary-condition.md) at $r=1$ term by term; the outer formula satisfies the condition at infinity. Each formula has its own stated region of validity, and the [matched asymptotic expansion](../../../../../matched-asymptotic-expansion.md) relates them in their overlap.

The constant can also be made explicit. [Integration by parts](../../../../../integration-by-parts.md) in the definition of $G$ gives $G=-EI-\int_x^\infty E(t)^2\,dt$, and $E(x)I(x)\to8$. Squaring the [complementary error function](../../../../../complementary-error-function.md) expression for $E$ separates the integral into three elementary pieces:

$$
\int_x^\infty E^2
=4\int_x^\infty\frac{e^{-2t}}t\,dt
-8\sqrt\pi\int_x^\infty\frac{e^{-t}}{\sqrt t}\operatorname{erfc}\sqrt t\,dt
+4\pi\int_x^\infty\operatorname{erfc}^2\sqrt t\,dt.
$$

The first piece is $-4\log x-4\gamma-4\log2+o(1)$, where $\gamma$ is the [Euler--Mascheroni constant](../../../../../euler-s-constant.md). Substitution $u=\sqrt t$ makes the second integral tend to $\sqrt\pi/2$, because $(\operatorname{erfc}u)'=-2e^{-u^2}/\sqrt\pi$. [Integration by parts](../../../../../integration-by-parts.md) in the third integral gives $1/2-1/\pi$. Consequently

$$
\boxed{\mu=4\gamma+4\log2+2\pi-4,\qquad
B=\frac{3\pi}{2}+\gamma+\log2-2.}
$$

Equivalently, defining $G$ by its convergent integral already determines the same matching constant without needing this closed form.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 82](../../paper-82-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
