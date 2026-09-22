<h1 id="1/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [range of the Volterra integration operator](../../../../../../../range-of-the-volterra-integration-operator.md) is $\{g\in H^1(0,1):g(0)=0\}$, using the representative of a [Sobolev space](../../../../../../../sobolev-space-split.md) element that is an [absolutely continuous function](../../../../../../../absolutely-continuous-function.md). Indeed $Ku$ has [weak derivative](../../../../../../../weak-derivative.md) $u$ and zero initial trace; conversely the [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) reconstructs such a $g$ from its derivative. This range contains smooth compactly supported functions and is dense in $L^2(0,1)$.

The given step is in $L^2$, and its value at the single midpoint is immaterial. It cannot be the image of an $L^2$ function: such an image is continuous, whereas no continuous representative agrees almost everywhere with zero on the left half and one on the right half. Its [distributional derivative](../../../../../../../distributional-derivative.md) is a [Dirac delta distribution](../../../../../../../dirac-delta-function.md), not an $L^2$ function. Thus

$$
\boxed{f\in\overline{\mathcal R(K)}\setminus\mathcal R(K).}
$$

For a direct approximation, replace the jump by a linear ramp of width $1/n$ centered at $1/2$. Each ramp starts at zero and has an $L^2$ derivative, so lies in the range, while its squared $L^2$ error is $1/(12n)$. Its derivative [norm](../../../../../../../norm.md) is $\sqrt n$, illustrating unstable differentiation.

The supplied [SVD](../../../../../../../singular-value-decomposition.md) gives $K(\sigma_j u_j)=\sigma_j^2v_j$, or more simply $K^\dagger(\sigma_jv_j)=u_j$. Since $\sigma_jv_j\to0$ but $\|u_j\|=1$, **the Moore–Penrose inverse is discontinuous**. Its domain is the dense, nonclosed range above, and there it is the [weak derivative](../../../../../../../weak-derivative.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
