<h1 id="14d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\theta=k\log t$. Since

$$
\dot x=\frac{\sin\theta+2k\cos\theta}{2k\sqrt t},
\qquad
\epsilon^{-2}=k^2+\frac14,
$$

the instantaneous oscillator energy is

$$
E(t)=\frac12\dot x^2+\frac{x^2}{2(\epsilon t)^2}
=\frac{1-\cos2\theta+2k\sin2\theta+4k^2}{8k^2t}.
$$

The instantaneous frequency is $\omega(t)=1/(\epsilon t)$, so

$$
I(t)=\frac{E(t)}{\omega(t)}
=\frac{\epsilon}{8k^2}\left(4k^2+1-\cos2\theta+2k\sin2\theta\right).
$$

Its oscillatory part divided by its mean is $O(k^{-1})=O(\epsilon)$. It remains bounded and periodic in $\log t$, so the variations do not accumulate. This is the expected behavior of an [adiabatic invariant](../../../../../../adiabatic-invariance-of-the-action.md): slow parameter variation produces small bounded oscillations rather than secular drift.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14D](../../14d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
