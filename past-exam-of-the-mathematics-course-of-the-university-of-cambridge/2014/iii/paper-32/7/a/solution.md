<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $r=\theta_A+\theta_B$, with $\theta_A\ge0$, $\theta_B>0$ and a finite $\tau\ge0$. The [competing risks model with transient surgical mortality](../../../../../../competing-risks-model-with-transient-surgical-mortality.md) has [survival function](../../../../../../survival-function.md)

$$
S(t)=\exp\{-\theta_Bt-\theta_A\min(t,\tau)\}.
$$

Integrating the disease [cause-specific hazard](../../../../../../cause-specific-hazard.md) against this [survival function](../../../../../../survival-function.md) gives

$$
\boxed{F_B(t)=\begin{cases}\dfrac{\theta_B}{r}(1-e^{-rt}),&0\le t\le\tau,\\[4pt]\dfrac{\theta_B}{r}(1-e^{-r\tau})+e^{-r\tau}\bigl(1-e^{-\theta_B(t-\tau)}\bigr),&t>\tau.\end{cases}}
$$

The first term accounts for disease deaths while both causes act; the second includes survivors of that period who then face only disease mortality. The [probability](../../../../../../probability.md) of eventually dying from surgery is

$$
\boxed{P(J=A)=F_A(\infty)=\int_0^\tau\theta_Ae^{-ru}\,du=\frac{\theta_A}{r}(1-e^{-r\tau}).}
$$

Taking the limit in $F_B$ gives $F_B(\infty)=\theta_B(1-e^{-r\tau})/r+e^{-r\tau}$, and therefore

$$
\boxed{F_A(\infty)+F_B(\infty)=1,\qquad S(\infty)=0.}
$$

The ultimate-death conclusion uses the positive continuing disease hazard. If $\theta_B=0$, the surviving fraction $e^{-\theta_A\tau}$ would instead live indefinitely in this model; the asserted conclusion is not valid in that boundary case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
