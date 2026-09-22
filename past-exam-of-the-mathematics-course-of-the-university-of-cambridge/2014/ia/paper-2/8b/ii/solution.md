<h1 id="8b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [small-angle approximation](../../../../../../small-angle-approximation.md) replaces $\sin\theta$ by $\theta$, giving the [damped harmonic oscillator](../../../../../../damped-harmonic-oscillator.md) equation $\ddot\theta+c\dot\theta+\theta=0$. Its [characteristic roots](../../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) satisfy $r^2+cr+1=0$.

For **$0<c<2$**, put $\nu=\sqrt{1-c^2/4}$; the motion is underdamped:

$$
\boxed{\theta(t)\simeq e^{-ct/2}[A\cos(\nu t)+B\sin(\nu t)].}
$$

It oscillates with decaying amplitude. For **$c=2$**, the repeated root gives [critical damping](../../../../../../critical-damping.md):

$$
\boxed{\theta(t)\simeq(A+Bt)e^{-t}.}
$$

For **$c>2$**, the motion is overdamped:

$$
\boxed{\theta(t)\simeq A e^{(-c+\sqrt{c^2-4})t/2}+B e^{(-c-\sqrt{c^2-4})t/2}.}
$$

Both real exponents are negative, so there is no oscillatory factor. The two constants are arbitrary in each case; these approximations require the displacement to remain small.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
