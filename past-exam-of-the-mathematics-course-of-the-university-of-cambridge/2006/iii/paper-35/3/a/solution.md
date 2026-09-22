<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $W$ is continuous and [adapted](../../../../../../adapted-process.md), the Borel function $\operatorname{sgn}(W)$ is [predictable](../../../../../../predictable-process.md). Its value at zero is $-1$, so its square is exactly one everywhere. Consequently $A$ is a zero-starting [continuous local martingale](../../../../../../continuous-local-martingale.md) with

$$
[A]_t=\int_0^t\operatorname{sgn}(W_s)^2ds=t.
$$

The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) therefore makes $A$ a [Brownian motion](../../../../../../brownian-motion-split.md) in the same [filtration](../../../../../../filtration-probability-theory.md). Here that characterization is the deterministic-clock case of the conditional-exponential argument in question 2.

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $V=W^2$:

$$
dV_t=2W_t\,dW_t+dt.
$$

Since $\sqrt{V_t}=|W_t|$ and $|W_t|\operatorname{sgn}(W_t)=W_t$, including at zero, substitution yields

$$
\boxed{dV_t=2\sqrt{V_t}\,dA_t+dt.}
$$

Thus $W^2$ is a [squared Bessel process](../../../../../../squared-bessel-process.md) of dimension one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
