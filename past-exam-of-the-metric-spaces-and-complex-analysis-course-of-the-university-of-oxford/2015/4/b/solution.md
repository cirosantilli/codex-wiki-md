<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $z\in\mathbb C\setminus[1,\infty)$, the number $w=1-z$ avoids the nonpositive [real axis](../../../../real-axis.md). Define the [branch of the complex logarithm](../../../../branch-of-the-complex-logarithm.md) by

$$
\boxed{L(1-z)=\log|1-z|+i\operatorname{Arg}(1-z),\qquad -\pi<\operatorname{Arg}(1-z)<\pi.}
$$

Here the [principal argument](../../../../principal-argument.md) is selected as a [continuous map](../../../../continuous-map.md) on that slit [domain](../../../../domain-mathematical-analysis.md), so this is a [holomorphic function](../../../../holomorphic-function-split.md), with [derivative](../../../../derivative.md) $-1/(1-z)$ and $L(1)=0$. For example, locally writing $w=\rho e^{i\phi}$ gives $d(\log\rho+i\phi)=dw/w$, verifying the [complex derivative](../../../../complex-derivative.md). The normalization also makes this [branch of the complex logarithm](../../../../branch-of-the-complex-logarithm.md) unique: any two continuous choices differ by a constant integer multiple of $2\pi i$ on the [connected](../../../../connected-space.md) slit [domain](../../../../domain-mathematical-analysis.md), and their values at $w=1$ agree.

To evaluate the corresponding [analytic branch of a square root](../../../../analytic-branch-of-a-square-root.md) on the [unit circle](../../../../complex-unit-circle.md), factor

$$
1-e^{i\theta}=e^{i\theta/2}\bigl(e^{-i\theta/2}-e^{i\theta/2}\bigr)=2\sin(\theta/2)e^{i(\theta/2-\pi/2)}.
$$

For $0<\theta<2\pi$, we have $\sin(\theta/2)>0$ and $-\pi/2<\theta/2-\pi/2<\pi/2$. Thus this factorization already uses the selected [principal argument](../../../../principal-argument.md), with no hidden change by $2\pi$. It follows that

$$
L(1-e^{i\theta})=\log\bigl(2\sin(\theta/2)\bigr)+i(\theta/2-\pi/2).
$$

Halving this expression and applying the [exponential function](../../../../exponential-function.md) gives

$$
\sqrt{1-e^{i\theta}}=\sqrt{2\sin(\theta/2)}\,e^{i\theta/4-i\pi/4}.
$$

Since $\sqrt2e^{-i\pi/4}=1-i$, the desired branch value is

$$
\boxed{\sqrt{1-e^{i\theta}}=(1-i)\sqrt{\sin(\theta/2)}\,e^{i\theta/4},\qquad 0<\theta<2\pi.}
$$

For instance, $\theta=\pi$ gives $\sqrt2>0$, a quick check that the sign agrees with the normalization.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
