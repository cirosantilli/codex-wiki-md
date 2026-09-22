<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Again put $T=\epsilon t$. To leading order the oscillator has form $x_0=k-r(T)\cos(t+\phi(T))$, while the second variable has a slow part $Y(T)$. Averaging its equation over the fast period gives

$$
Y_T=1+k-Y,\qquad Y(0)=0,
\qquad \boxed{Y(T)=(1+k)(1-e^{-T})}.
$$

The oscillatory forcing of the second variable produces only an order-$\epsilon$ correction: its leading fast [derivative](../../../../../../../derivative.md) is $-r(T)\cos t$, whose bounded primitive is $-r(T)\sin t$. Thus it creates no [secular term](../../../../../../../secular-term.md).

The oscillator [solvability condition](../../../../../../../solvability-condition.md) is the same as in part (i), with $c$ replaced by $Y(T)$:

$$
r_T=\frac Y2(k^2-1)r+\frac Y8r^3,\qquad\phi_T=0.
$$

Introduce accumulated [slow time](../../../../../../../slow-time.md)

$$
S(T)=\int_0^T Y(s)\,ds=(1+k)(T-1+e^{-T}).
$$

The [shifted Van der Pol amplitude evolution](../../../../../../../shifted-van-der-pol-amplitude-evolution.md) therefore gives, for $a=k^2-1$,

$$
r^2(T)=\frac{k^2e^{aS(T)}}{1-\dfrac{k^2}{4a}(e^{aS(T)}-1)}\quad(a\ne0),\qquad
r(T)=[1-S(T)/4]^{-1/2}\quad(k=1).
$$

Consequently

$$
\boxed{x(t)=k-r(\epsilon t)\cos t+O(\epsilon),\qquad
y(t)=(1+k)(1-e^{-\epsilon t})+O(\epsilon)}.
$$

As before, uniformity for $t=O(\epsilon^{-1})$ means a fixed bounded slow-time interval on which the envelope stays bounded. For $k^2>4/5$ it fails when $S(T)$ reaches $\log(5-4/k^2)/(k^2-1)$, with limiting value $4$ at $k=1$. There is no bounded leading approximation covering all such slow times for arbitrary positive $k$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
