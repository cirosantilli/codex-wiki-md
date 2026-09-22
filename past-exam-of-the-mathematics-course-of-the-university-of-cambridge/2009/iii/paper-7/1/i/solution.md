<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and normalized [Haar measure](../../../../../../haar-measure.md) $dm=ds\,dt/(2\pi)^2$ on the [torus](../../../../../../torus.md). Here $|s|$ means distance to zero modulo $2\pi$, represented in $[-\pi,\pi]$; an ordinary coordinate in $[0,2\pi)$ would not express concentration at the origin correctly.

Put $B(s,t)=2+\cos s+\cos t$, $I_N=\int B^Ndm$, and $A_N=I_N^{-1}$. Since $0\le B\le4$ and $B(0,0)=4$, $I_N>0$, the kernel $K_N=A_NB^N$ is nonnegative, and $\int K_Ndm=1$ exactly. Fix $0<\delta\le\pi$. On the set where either $|s|\ge\delta$ or $|t|\ge\delta$, $B\le q=3+\cos\delta<4$. Choose $q'$ with $q<q'<4$. [continuity](../../../../../../continuous-function.md) provides a neighborhood $U$ of the origin of positive measure $v$ where $B\ge q'$. Consequently

$$
I_N\ge v(q')^N,\qquad\sup_{\max(|s|,|t|)\ge\delta}K_N(s,t)\le\frac1v\left(\frac q{q'}\right)^N\longrightarrow0.
$$

For $0<\varepsilon\le\pi$, take $\delta=\varepsilon$ and then $N$ large enough that this bound is at most $\varepsilon$. For $\varepsilon>\pi$ the exterior conditions are empty. This proves all the requested kernel properties, with $\boxed{A=\left[\int(2+\cos s+\cos t)^Ndm\right]^{-1}}$.

Now let $M=\|f\|_\infty$ and define $P_N=K_N*f$. The [powered-cosine approximate identity on a torus](../../../../../../powered-cosine-approximate-identity-on-a-torus.md) is a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md), since its base is a finite sum of [complex exponentials](../../../../../../complex-exponential-function.md) and its exponent is an integer. Expanding $K_N$ and integrating its finitely many Fourier terms shows that $P_N$ is also a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md); it is real-valued because both factors are real. Translation invariance and normalization give

$$
P_N(x,y)-f(x,y)=\int K_N(s,t)[f(x-s,y-t)-f(x,y)]dm(s,t).
$$

Given $\eta>0$, [uniform continuity](../../../../../../uniform-continuity.md) of $f$ supplies $\delta>0$ making the difference in brackets smaller than $\eta/2$ on the square $|s|,|t|<\delta$, uniformly in $(x,y)$. The contribution from that square is at most $\eta/2$. On its complement it is at most $2M\sup_{\max(|s|,|t|)\ge\delta}K_N$, which tends to zero by the preceding estimate. Therefore $\boxed{\|P_N-f\|_\infty\to0}$, proving uniform approximation without assuming any Fourier-series convergence of $f$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
