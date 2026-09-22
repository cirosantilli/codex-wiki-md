<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $T=\epsilon t$ and use the [method of multiple scales](../../../../../../../method-of-multiple-scales.md) with $x=x_0(t,T)+\epsilon x_1+\cdots$. At leading order, $x_{0,tt}+x_0=k$, so write $x_0=k-r(T)\cos(t+\phi(T))$ with $r(0)=k$, $\phi(0)=0$. The order-$\epsilon$ equation is

$$
(\partial_t^2+1)x_1=-2\partial_t\partial_Tx_0-c(1-x_0^2)\partial_tx_0.
$$

Using $\cos^2 t\sin t=(\sin t+\sin3t)/4$, its fundamental sine coefficient is $-2r_T-c r(1-k^2-r^2/4)$, and its fundamental cosine coefficient forces $\phi_T=0$. Removing these resonant forcings is the [solvability condition in the method of multiple scales](../../../../../../../solvability-condition-in-the-method-of-multiple-scales.md). Thus the [shifted Van der Pol amplitude evolution](../../../../../../../shifted-van-der-pol-amplitude-evolution.md) is

$$
\boxed{r_T=\frac c2(k^2-1)r+\frac c8r^3,\qquad \phi_T=0}.
$$

With $a=k^2-1$ and $R=r^2$, solve $R_T=caR+cR^2/4$ by putting $W=1/R$. This gives

$$
\boxed{r^2(T)=\frac{k^2e^{caT}}{1-\dfrac{k^2}{4a}(e^{caT}-1)}}\quad(a\ne0),\qquad
\boxed{r(T)=(1-cT/4)^{-1/2}}\quad(k=1).
$$

The uniformly valid leading approximation is **$x(t)=k-r(\epsilon t)\cos t+O(\epsilon)$** on bounded slow-time intervals for which $r$ remains bounded. The exact initial [derivative](../../../../../../../derivative.md) is recovered by the first-order correction; the displayed leading expression already satisfies the leading initial data.

There is an important limitation to the source's unqualified time-range wording. Starting from $r(0)=k$, the [amplitude](../../../../../../../wave-amplitude.md) decays for $k^2<4/5$, is constant at leading order for $k^2=4/5$, and grows for $k^2>4/5$. In the latter case the denominator vanishes at

$$
T_b=\frac{\log(5-4/k^2)}{c(k^2-1)},\qquad T_b=4/c\ \text{when }k=1.
$$

A bounded-amplitude [multiple-scale expansion](../../../../../../../method-of-multiple-scales.md) is uniform for $0\le T\le C<T_b$, not through its predicted large-amplitude breakdown. For the decaying case every fixed bounded slow-time interval is available; the leading unstable equilibrium at $k^2=4/5$ also has bounded [amplitude](../../../../../../../wave-amplitude.md) over such intervals. The envelope singularity is a breakdown warning, not a proof that the exact original solution has precisely this blow-up time. The coefficient in the PDF is $\epsilon c$, correcting the converted TeX's duplicated $\epsilon$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
