<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [annual pulse-breeding predator-prey model](../../../../../../annual-pulse-breeding-predator-prey-model.md). Let $X_n,Y_n$ be the abundances just after reproduction, and let the year have length $T$. Between breeding pulses, assume mass-action [predation](../../../../../../predation.md), natural mortality rates $\mu_X,\mu_Y>0$, and no reproduction:

$$
\dot X=-\mu_XX-\beta XY,\qquad \dot Y=-\mu_YY.
$$

Solving the [predator](../../../../../../predator.md) equation and inserting it into the [prey](../../../../../../prey.md) equation gives the pre-breeding abundances

$$
Y^-_n=e^{-\mu_YT}Y_n,
\qquad
X^-_n=X_n\exp\!\left[-\mu_XT-
\frac{\beta(1-e^{-\mu_YT})}{\mu_Y}Y_n\right].
$$

Suppose reproduction multiplies surviving [prey](../../../../../../prey.md) by $R$ and adds $qX^-_n$ offspring per surviving [predator](../../../../../../predator.md). Retaining the surviving adults gives $X_{n+1}=RX^-_n$, $Y_{n+1}=Y^-_n(1+qX^-_n)$. Define $r=Re^{-\mu_XT}$, $s=e^{-\mu_YT}$, $\kappa=\beta(1-s)/\mu_Y$ and $b=q/R$. The resulting [difference equations](../../../../../../difference-equation.md) are

$$
\boxed{X_{n+1}=rX_ne^{-\kappa Y_n},\qquad
Y_{n+1}=sY_n(1+bX_{n+1}).}
$$

Thus offspring depend on [prey](../../../../../../prey.md) available at the end of the year, not on the number killed during the year. The adult-survival convention is part of the model; if breeding replaces all adults, use $Y_{n+1}=sbY_nX_{n+1}$ instead. Both are consistent pulse models under their respective life-history assumptions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
