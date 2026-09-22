<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Gronwall inequality](../../../../../../gronwall-inequality.md) applied to part (a) gives

$$
\boxed{\mathbb E f_\epsilon(Z_{t\wedge\tau})\leq\frac{e^{(L+K^2)t}}{z_0+\epsilon}.}
$$

Continuity implies $Z_\tau=0$ on $\{\tau<\infty\}$. Thus on $\{\tau\leq t\}$ the stopped reciprocal equals $1/\epsilon$. Positivity gives

$$
\mathbb P(\tau\leq t)\leq\epsilon\mathbb E f_\epsilon(Z_{t\wedge\tau})\leq\frac\epsilon{z_0+\epsilon}e^{(L+K^2)t}.
$$

Let $\epsilon\downarrow0$, using $z_0>0$, to obtain $\mathbb P(\tau\leq t)=0$. Taking the union over integer $t$ proves $\tau=\infty$ almost surely. Hence the [strict order preservation for scalar Lipschitz diffusions](../../../../../../strict-order-preservation-for-scalar-lipschitz-diffusions.md) conclusion is

$$
\boxed{\mathbb P(X_t<Y_t\text{ for every }t\geq0)=1,}
$$

which is stronger than the requested weak inequality. The single-event argument prevents a gap between fixed-time ordering and simultaneous ordering at all times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
