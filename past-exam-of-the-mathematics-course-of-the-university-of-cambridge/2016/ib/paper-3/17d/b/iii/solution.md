<h1 id="17d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $B_0\ne0$, [Newton's second law](../../../../../../../newton-s-second-law.md) gives

$$
m\ddot s=\frac{B_0L\mathcal E_0}{R}-\frac{B_0^2L^2}{R}\dot s.
$$

Define the [exponential relaxation time](../../../../../../../exponential-relaxation-time.md) $\tau=mR/(B_0^2L^2)$ and [terminal velocity](../../../../../../../terminal-velocity.md) $v_\infty=\mathcal E_0/(B_0L)$. Solving the first-order equation for $v=\dot s$ and then integrating gives

$$
\boxed{\dot s(t)=v_\infty+(v_0-v_\infty)e^{-t/\tau},\qquad
s(t)=s_0+v_\infty t+\tau(v_0-v_\infty)(1-e^{-t/\tau}).}
$$

Both prescribed initial values hold. The current approaches zero as the bar approaches terminal velocity. If $B_0=0$, there is no magnetic force and instead $\dot s=v_0$, $s=s_0+v_0t$; the constant current is $\mathcal E_0/R$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [17D](../../../17d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
