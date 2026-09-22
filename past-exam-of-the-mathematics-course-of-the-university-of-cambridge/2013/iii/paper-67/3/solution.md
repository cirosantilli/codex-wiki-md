<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume $\epsilon\to0^+$. Since the drift $(1+x)^2$ is positive, the fast mode decays to the right; the [matched asymptotic expansion](../../../../../matched-asymptotic-expansion.md) has a left [boundary layer](../../../../../boundary-layer.md) at $x=0$ of width $O(\epsilon)$, and the [outer expansion](../../../../../outer-expansion.md) uses the condition at $x=1$.

Write $y\sim y_0+\epsilon y_1$. The first two equations for the [outer expansion](../../../../../outer-expansion.md) are

$$
(1+x)^2y_0'+y_0=0,\qquad (1+x)^2y_1'+y_1=-y_0''.
$$

Enforcing $y_0(1)=1$ and $y_1(1)=0$, define

$$
E(x)=e^{1/(1+x)-1/2},\qquad
q(x)=\frac1{2(1+x)^4}+\frac1{5(1+x)^5}-\frac3{80}.
$$

Then the outer [asymptotic expansion](../../../../../asymptotic-expansion.md) is

$$
\boxed{y_{\rm out}(x)=E(x)\left[1+\epsilon q(x)\right]+O(\epsilon^2)}.
$$

To derive the correction, set $y_1=E q$. Cancellation of the homogeneous terms leaves $q'=-2/(1+x)^5-1/(1+x)^6$; integration and $q(1)=0$ give the expression above.

In the left [boundary layer](../../../../../boundary-layer.md), set $\xi=x/\epsilon$ and $y=Y_0(\xi)+\epsilon Y_1(\xi)+\cdots$. The equation becomes $Y''+(1+\epsilon\xi)^2Y'+\epsilon Y=0$. Put $A=e^{1/2}$ and $B=1-A$. The leading inner equation and matching give $Y_0''+Y_0'=0$, $Y_0(0)=1$, $Y_0(\infty)=A$, hence $Y_0=A+B e^{-\xi}$. At the next order,

$$
Y_1''+Y_1'=-2\xi Y_0'-Y_0=-A+B(2\xi-1)e^{-\xi}.
$$

Since $q(0)=53/80$, put $C=53A/80$. The matched inner correction satisfying $Y_1(0)=0$ is

$$
\boxed{Y_1=-A\xi+C(1-e^{-\xi})-B(\xi^2+\xi)e^{-\xi}}.
$$

For verification, the differential operator $d^2/d\xi^2+d/d\xi$ maps $e^{-\xi}P(\xi)$ to $e^{-\xi}(P''-P')$. The large-$\xi$ common part is $A+\epsilon(C-A\xi)$, precisely the small-$x$ [outer expansion](../../../../../outer-expansion.md) in the overlap $\epsilon\ll x\ll1$.

Adding the [inner expansions](../../../../../inner-expansion.md) and [outer expansions](../../../../../outer-expansion.md) and subtracting their common part gives the [first-order composite expansion for a positive drift](../../../../../first-order-composite-expansion-for-a-positive-drift.md)

$$
\boxed{y_{\rm comp}(x)=E(x)[1+\epsilon q(x)]+e^{-x/\epsilon}\left[B-\epsilon C-\epsilon B\left(\frac{x^2}{\epsilon^2}+\frac{x}{\epsilon}\right)\right]}.
$$

This is uniformly correct through $O(\epsilon)$ on $0\leq x\leq1$. It satisfies the left [boundary condition](../../../../../boundary-condition.md) exactly; at the right boundary the remaining error is exponentially small. Polynomial growth in the inner correction is harmless because it is multiplied by the decaying exponential. For the smooth nonvanishing drift, the next matched terms are uniformly $O(\epsilon^2)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
