<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The printed assumptions omit the orthogonality needed for the claimed local martingales.** Merely placing two [Brownian motions](../../../../../../brownian-motion-split.md) on the same [probability space](../../../../../../probability-space.md) does not make them independent. Interpret both as [Brownian motions](../../../../../../brownian-motion-split.md) relative to a common [filtration](../../../../../../filtration-probability-theory.md), and put $C_t=[B,\vartheta]_t$. For $X=e^B\cos\vartheta$ and $Y=e^B\sin\vartheta$, the two-variable [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
\boxed{dX=X\,dB-Y\,d\vartheta-Y\,dC,\qquad dY=Y\,dB+X\,d\vartheta+X\,dC.}
$$

The pure second derivatives cancel because $[B]_t=[\vartheta]_t=t$, while the mixed [partial derivatives](../../../../../../partial-derivative.md) are $X_{b\vartheta}=-Y$ and $Y_{b\vartheta}=X$. Thus the mixed [quadratic covariation](../../../../../../quadratic-covariation.md) term cannot be omitted.

For a counterexample allowed by the PDF, take $\vartheta=B$. Then $C_t=t$ and $X$ has drift $-Y\,dt$, while $Y$ has drift $X\,dt$. In particular $X_0=1$ makes the latter drift nonzero near zero, so $Y$ is not a [local martingale](../../../../../../local-martingale.md). Nor is $X$: $Y$ cannot be identically zero, so its accumulated continuous drift is not identically zero. Uniqueness of the [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) excludes cancellation by another [local martingale](../../../../../../local-martingale.md) term.

The corrected hypothesis is $[B,\vartheta]\equiv0$, for example independent [Brownian motions](../../../../../../brownian-motion-split.md) in their joint [filtration](../../../../../../filtration-probability-theory.md). Conversely, if both were [local martingales](../../../../../../local-martingale.md), uniqueness of the [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) would force $Y\,dC=X\,dC=0$; since $X^2+Y^2=e^{2B}>0$, this forces $dC=0$. Thus the correction is exactly the condition needed for both [local martingales](../../../../../../local-martingale.md). Under this hypothesis the drift terms vanish and the intended [stochastic differential equations](../../../../../../stochastic-differential-equation.md) are $dX=X\,dB-Y\,d\vartheta$ and $dY=Y\,dB+X\,d\vartheta$. The continuous integrands are locally bounded, so localization makes these [Itô integrals](../../../../../../ito-integral.md) [continuous local martingales](../../../../../../continuous-local-martingale.md). Subsequent intended conclusions are proved under this explicitly stated correction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
