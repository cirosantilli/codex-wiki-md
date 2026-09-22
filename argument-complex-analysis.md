# Argument (complex analysis)

↑ **Parent:** [Complex number](complex-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Argument_(complex_analysis))

An [argument](argument-complex-analysis.md) of a nonzero [complex number](complex-number.md) $z$ is any [angle](angle.md) $\theta$ for which $z=|z|e^{i\theta}$. All [arguments](argument-complex-analysis.md) are $\theta+2\pi k$, with $k$ an [integer](integer-split.md). Zero has no [argument](argument-complex-analysis.md): it has no distinguished direction. A commonly chosen representative, the principal [argument](argument-complex-analysis.md) $\operatorname{Arg}z$, lies in $(-\pi,\pi]$. Choosing representatives is part of specifying a [branch of a multivalued function](branch-of-a-multivalued-function.md). These conventions are described in [Jeremy Orloff, MIT 18.04, topic 1, sections 1.5 and 1.14](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/6eae09885b0fab3f068e31752198abea_MIT18_04S18_topic1.pdf).

For $3+4i$, the principal [argument](argument-complex-analysis.md) is $\arctan(4/3)\approx0.927295$ [radians](radian.md), computed with the [inverse tangent](inverse-tangent.md). But the coordinate ratio alone loses the quadrant: $-3-4i$ has the same ratio $4/3$, yet its principal [argument](argument-complex-analysis.md) is $\arctan(4/3)-\pi\approx-2.214297$ [radians](radian.md).

For nonzero $z,w$, the correct rule is

$$
\operatorname{Arg}(zw)\equiv\operatorname{Arg}z+\operatorname{Arg}w\pmod{2\pi}.
$$

Ordinary equality can fail. With $z=w=e^{3\pi i/4}$, their principal [arguments](argument-complex-analysis.md) sum to $3\pi/2$, but $zw=-i$ has principal [argument](argument-complex-analysis.md) $-\pi/2$. They differ by one full turn. As a point crosses the negative horizontal axis, the principal [argument](argument-complex-analysis.md) jumps by $2\pi$. A continuous choice on a suitable region therefore requires a [branch cut](branch-cut.md); the jump belongs to the choice of representative, although the point moves smoothly.

**Table of contents**

- [Principal argument](principal-argument.md)

## ↑ Ancestors (6)

1. [Complex number](complex-number.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
