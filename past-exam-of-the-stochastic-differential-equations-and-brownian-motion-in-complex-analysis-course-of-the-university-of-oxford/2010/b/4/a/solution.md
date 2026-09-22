<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a printed domain error: $\operatorname{Re}z>0$ defines the right half-plane. Taken literally, continuity forces $\operatorname{Re}Z_{T_H}=0$ almost surely, so its law is a point mass at zero. The displayed density belongs to the intended upper half-plane $\operatorname{Im}z>0$, with $b>0$. We prove that intended assertion explicitly.

Write $Z_t=a+X_t+i(b+Y_t)$ for independent standard [Brownian motions](../../../../../brownian-motion-split.md). The exit time $T$ is the first time $Y$ hits $-b$, and depends only on $Y$. Its density, by the supplied [Brownian first-passage time](../../../../../brownian-first-passage-time.md) law, is $b(2\pi t^3)^{-1/2}e^{-b^2/(2t)}$. Conditional on $T=t$, the real exit coordinate is [normally distributed](../../../../../normal-distribution.md) with mean $a$ and variance $t$. Independence therefore gives

$$
h(x)=\frac b{2\pi}\int_0^\infty t^{-2}
\exp\left(-\frac{b^2+(x-a)^2}{2t}\right)dt.
$$

With $u=[b^2+(x-a)^2]/(2t)$, the integral is $2/[b^2+(x-a)^2]$. Thus the [Cauchy exit law from a Brownian half-plane](../../../../../cauchy-exit-law-from-a-brownian-half-plane.md) is

$$
\boxed{h(x)=\frac b{\pi[b^2+(x-a)^2]}.}
$$

For the literal right half-plane, the corresponding nondegenerate coordinate is $\operatorname{Im}Z_{T_H}$, whose density is $a/\{\pi[a^2+(y-b)^2]\}$ for $a>0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
