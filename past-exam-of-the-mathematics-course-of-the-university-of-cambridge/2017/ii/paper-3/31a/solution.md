<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

With the sign convention of the displayed operator, the [Lax equation](../../../../../isospectral-lax-equation.md) is $L_t=[L,A]$. Differentiating $L\varphi=k^2\varphi$ shows that $\varphi_t+A\varphi$ is another solution at the same spectral parameter. The normalization at $-\infty$ fixes

$$
 \varphi_t=-A\varphi+4ik^3\varphi,
$$

since $A e^{-ikx}=4ik^3e^{-ikx}$ there. At $+\infty$, comparison of the two plane-[wave](../../../../../wave.md) coefficients gives

$$
\boxed{a_t=0,\qquad b_t=8ik^3b,\qquad b(k,t)=b(k,0)e^{8ik^3t}.}
$$

Thus the transmission denominator $a$ is time independent. This is the [Time evolution of KdV scattering data](../../../../../time-evolution-of-kdv-scattering-data.md) for the stated normalization.

The [logarithmic derivative](../../../../../logarithmic-derivative.md) $S=\varphi_x/\varphi+ik$ obeys the [Riccati equation](../../../../../riccati-equation.md)

$$
 S'-2ikS+S^2=u.
$$

Its formal large-$k$ expansion gives

$$
 S_1=-u,\qquad S_{n+1}=S_n'+\sum_{j=1}^{n-1}S_jS_{n-j},\qquad
 S_2=-u',\quad S_3=-u''+u^2,\quad S_4=-u'''+4uu'.
$$

There is an important qualification to the [integral](../../../../../integral.md) identity in the question. For real $k$ with nonzero reflection, $e^{ikx}\varphi\sim a+b e^{2ikx}$ has no [limit](../../../../../limit-of-a-function.md) at $+\infty$, so the literal improper [integral](../../../../../integral.md) of the exact $S$ need not exist. Continue to $\operatorname{Im}k>0$, where the reflected exponential decays relative to $e^{-ikx}$, and take sufficiently large $k$ away from zeros and with a consistent [logarithm](../../../../../logarithm.md). Then the normalization gives

$$
\boxed{a(k,t)=\exp\left(\int_{-\infty}^{\infty}S(x,k,t)\,dx\right),\qquad
 \log a\sim\sum_{n\geq1}\frac{\int S_n\,dx}{(2ik)^n}.}
$$

The second equality is an [asymptotic expansion](../../../../../asymptotic-expansion.md), not an asserted convergent [series](../../../../../series-mathematics.md). Time independence of $a$ fixes every coefficient, so each $\int S_n dx$ is a [conserved quantity](../../../../../conserved-quantity.md) of the [Korteweg-De Vries equation](../../../../../korteweg-de-vries-equation.md). The first two nontrivial examples are $-\int u dx$ and $\int u^2dx$.

For the usual real-valued KdV potential and real formal $k$, write $S=X+iY$ with real coefficient functions. Its imaginary part of the [Riccati equation](../../../../../riccati-equation.md) is $Y'-2kX+2XY=0$, hence

$$
 X=\frac{Y'}{2(k-Y)}=-\frac12\partial_x\log(1-Y/k).
$$

In the formal expansion, $X$ contains precisely the even-indexed $S_n$ and $Y$ the odd-indexed ones. Rapid decay of $u$ and its [derivatives](../../../../../derivative.md) makes every coefficient of the [logarithm](../../../../../logarithm.md) vanish at both spatial ends. Therefore $\boxed{\int_{\mathbb R}S_{2j}\,dx=0\quad(j\geq1)}$. This is a coefficientwise formal identity; it does not claim that the exact real-axis reflected solution has a convergent [integral](../../../../../integral.md) of $X$. The analytically continued scattering identity and the formal expansion are the conventions needed to make the requested argument valid.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
