<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Continue with $A_d$ equal to the integral defined in the PDF and $u(z)=|z|^{2-d}$. Until the [Brownian motion](../../../../../../brownian-motion-split.md) hits the radius-$\varepsilon$ ball, $u(B_s)$ is a bounded [local martingale](../../../../../../local-martingale.md), hence a true [martingale](../../../../../../martingale-split.md). At the finite [stopping time](../../../../../../stopping-time.md) $t\wedge T_\varepsilon$, [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
u(x)=\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)+\mathbb E_x[u(B_t);T_\varepsilon>t].
$$

Rearranging,

$$
\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)
=u(x)-\mathbb E_xu(B_t)+\mathbb E_x[u(B_t);T_\varepsilon\leq t].
$$

The fixed random variable $u(B_t)$ is integrable by the [Gaussian heat kernel](../../../../../../gaussian-heat-kernel.md) and the local-integrability calculation above. Also $\mathbb P_x(T_\varepsilon\leq t)\leq(\varepsilon/|x|)^{d-2}\to0$. For any $R>0$, the final [expectation](../../../../../../expected-value.md) is at most

$$
\mathbb E_x[u(B_t);u(B_t)>R]+R\mathbb P_x(T_\varepsilon\leq t).
$$

First send $\varepsilon\downarrow0$, then $R\to\infty$, proving that it vanishes. The identities from part (b) give

$$
u(x)=A_d^{-1}\int_0^\infty p(s,0,x)ds,\qquad
\mathbb E_xu(B_t)=A_d^{-1}\int_t^\infty p(s,0,x)ds.
$$

Subtracting yields the [small-ball Brownian hitting asymptotic](../../../../../../small-ball-brownian-hitting-asymptotic.md)

$$
\boxed{\lim_{\varepsilon\downarrow0}\varepsilon^{2-d}\mathbb P_x(T_\varepsilon\leq t)
=A_d^{-1}\int_0^t p(s,0,x)\,ds.}
$$

Thus the constant in this printed limit requires exactly the same reciprocal correction as in part (b). For $d=3$ the multiplier is $2\pi$, not $1/(2\pi)$. The argument proves the corrected finite-time limit directly, rather than inferring it from the eventual hitting probability alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
