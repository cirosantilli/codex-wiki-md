<h1 id="a/1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Initially $a=1/2$ and $T=T_+/T_0>1$, so $\varepsilon T_t=1-T^4<0$. On the fast time $s=t/\varepsilon$, [albedo](../../../../../albedo.md) changes by only $O(\varepsilon)$ and

$$
T_s=1-T^4,\qquad T(0)=T_+/T_0.
$$

Thus [temperature](../../../../../temperature-split.md) rapidly falls towards $1$. At the same time $a_t=a^*(T)-1/2<0$ while $T>1$, which seeds selection of the warm branch. Afterwards the approximate [slow manifold](../../../../../slow-manifold.md) is $T^4=2(1-a)$: decreasing [albedo](../../../../../albedo.md) makes [temperature](../../../../../temperature-split.md) rise slowly back towards $T_+/T_0$. The preceding figure separates these two time scales; a single time axis would compress the initial fall into a nearly vertical segment.

In the sharp-transition regime, after selection of the warm branch $a^*(T)\simeq1/4$. Solving the linear [ordinary differential equation](../../../../../ordinary-differential-equation.md) with the leading matched value $a(0^+)=1/2$ gives

$$
\boxed{a(t)\simeq\frac14+\frac14e^{-t},\qquad T(t)\simeq\left(\frac{3-e^{-t}}2\right)^{1/4}.}
$$

These are [outer solutions](../../../../../outer-expansion.md): their initial [temperature](../../../../../temperature-split.md) is $1$, so the fast cooling layer is required to satisfy the actual initial [temperature](../../../../../temperature-split.md).

There is a useful qualification to the two-limit argument. For fixed finite $\mu>2$, put $x=1-2a$ on the [slow manifold](../../../../../slow-manifold.md). Then $x_t=-x+\tfrac12\tanh(\mu x)$, and $x=0$ is an unstable [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) with growth rate $\mu/2-1$. The small positive $O(\varepsilon)$ seed from the fast layer can therefore produce a delay of order $\log(1/\varepsilon)/(\mu/2-1)$. The simple exponential approximation assumes that the sharp [albedo](../../../../../albedo.md) transition is sufficiently fast to make this delay negligible on the displayed slow scale. It is not a uniform approximation for every fixed $\mu>2$ as $\varepsilon\to0$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
