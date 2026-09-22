<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $k$ is constant, as for constant resting long-wave speed. With $S_0'/S_0=\beta$, put $\eta=e^{-\beta x/2}Y$. The amplitude equation becomes

$$
Y''+\left(k^2-\frac{\beta^2}{4}\right)Y=0.
$$

If $k^2>\beta^2/4$, write $\mu=\sqrt{k^2-\beta^2/4}$: the solution is an oscillatory sine-cosine combination multiplied by $e^{-\beta x/2}$. If $k^2=\beta^2/4$, it is $e^{-\beta x/2}(A+Bx)$. If $k^2<\beta^2/4$, it is a combination of real exponentials, $e^{-\beta x/2}(Ae^{\gamma x}+Be^{-\gamma x})$, where $\gamma=\sqrt{\beta^2/4-k^2}$. These classify the local spatial behavior.

For a nonzero-frequency mode, zero velocity at both dams and $v_t=-g\eta_x$ impose $\eta'(0)=\eta'(L)=0$. In the oscillatory case, the first condition gives

$$
\eta=Ae^{-\beta x/2}\left[\cos\mu x+\frac{\beta}{2\mu}\sin\mu x\right].
$$

Its derivative at $L$ is $-Ak^2e^{-\beta L/2}\sin(\mu L)/\mu$. Hence the [standing modes in an exponentially tapered channel](../../../../../../standing-modes-in-an-exponentially-tapered-channel.md) have

$$
\boxed{\mu_n=\frac{n\pi}{L},\qquad
k_n^2=\left(\frac{n\pi}{L}\right)^2+\frac{\beta^2}{4},\qquad
\omega_n=c_0k_n,\quad n=1,2,\ldots.}
$$

The hyperbolic and repeated-root cases provide no additional nonzero-frequency mode satisfying both end conditions. There is a separate zero-frequency uniform-level mode $\eta=\mathrm{constant}$, corresponding to a change of the basin's conserved water volume.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
