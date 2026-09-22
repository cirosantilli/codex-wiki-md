<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The positive denominators in this part are **Euclidean**. Starting with the [Minkowski spacetime](../../../../minkowski-spacetime.md) [Feynman rules](../../../../feynman-rules.md), first perform a [Wick rotation](../../../../wick-rotation.md); a bare [Minkowski metric](../../../../minkowski-metric.md) integral without a pole prescription would not equal the displayed positive expression. Work initially with $m^2>0$ and $\Re n>D/2$, where the [Euclidean massive loop integral](../../../../euclidean-massive-loop-integral.md) converges.

Use [Schwinger parameterization](../../../../schwinger-parameterization.md) followed by the [Gaussian integral](../../../../gaussian-integral.md):

$$
\frac1{(k^2+m^2)^n}=\frac1{\Gamma(n)}\int_0^\infty ds\,s^{n-1}e^{-s(k^2+m^2)},
\qquad
\int\frac{d^Dk}{(2\pi)^D}e^{-sk^2}=\frac1{(4\pi s)^{D/2}}.
$$

The remaining [Gamma function](../../../../gamma-function.md) integral gives

$$
\begin{aligned}
I_{D,n}(m^2)
&=\frac1{(4\pi)^{D/2}\Gamma(n)}\int_0^\infty ds\,s^{n-D/2-1}e^{-sm^2}\\
&=\boxed{\frac{\Gamma(n-D/2)}{(4\pi)^{D/2}(n-1)!}(m^2)^{D/2-n}}.
\end{aligned}
$$

The factorial form is for positive integral $n$. [Dimensional regularization](../../../../dimensional-regularization.md) defines the result elsewhere by [analytic continuation](../../../../analytic-continuation.md).

For the [scalar bubble integral](../../../../scalar-bubble-integral.md), combine the two denominators with a [Feynman parameter](../../../../feynman-parameter.md) $x$ and shift the integration variable to $\ell=k-(1-x)p_E$. Then

$$
B_D(p_E)=\int_0^1dx\,I_{D,2}(M_x^2),
\qquad M_x^2=m^2+x(1-x)p_E^2.
$$

For $D=4-\epsilon$ this is

$$
B_D(p_E)=\frac{\Gamma(\epsilon/2)}{(4\pi)^{2-\epsilon/2}}\int_0^1dx\,(M_x^2)^{-\epsilon/2}.
$$

The [Gamma function](../../../../gamma-function.md) recurrence gives $\Gamma(\epsilon/2)=2/\epsilon+O(1)$, and the parameter integral is $1+O(\epsilon)$. Consequently

$$
\boxed{B_D(p_E)=\frac1{8\pi^2\epsilon}+O(1).}
$$

This [ultraviolet divergence](../../../../ultraviolet-divergence.md) is independent of the external [momentum](../../../../momentum-split.md). The assumption $m^2>0$ avoids an [infrared divergence](../../../../infrared-divergence.md). In particular the completely massless zero-momentum integral is a [scaleless integral](../../../../scaleless-integral.md) and vanishes in [dimensional regularization](../../../../dimensional-regularization.md); its ultraviolet and infrared poles must be separated before assigning it the displayed ultraviolet residue.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
