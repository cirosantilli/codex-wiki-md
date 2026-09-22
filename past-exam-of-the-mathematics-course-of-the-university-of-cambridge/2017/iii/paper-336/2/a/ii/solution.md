<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The small denominator lies near $x=0$ when $\gamma$ approaches $1$. Its two contributions balance when $\gamma-1=O(\varepsilon)$ and $x=O(\varepsilon)$. Let

$$
\gamma=1+\varepsilon\eta,\qquad x=\varepsilon s,\qquad L=\log2,
$$

with fixed real $\eta$. Then $1-\gamma+\gamma x=\varepsilon(s-\eta)+O(\varepsilon^2)$ and $\log(2-x)=L+O(\varepsilon s)$ in the contributing region. The [endpoint transition of a regularized interior pole](../../../../../../../endpoint-transition-of-a-regularized-interior-pole.md) gives

$$
\boxed{I(1+\varepsilon\eta;\varepsilon)\sim\frac1{\varepsilon L}\left[\frac\pi2+\arctan\left(\frac\eta L\right)\right].}
$$

Indeed, the leading scaled [integral](../../../../../../../integral.md) is $\varepsilon^{-1}\int_0^\infty[(s-\eta)^2+L^2]^{-1}ds$. The upper endpoint can be sent to infinity at leading order because the omitted tail contributes only $O(1)$ to the original [integral](../../../../../../../integral.md). At $\gamma=1$ the result is $\pi/(2\varepsilon\log2)$: only one half of the narrow peak lies in the domain.

This formula provides the required matching. For $\eta\to-\infty$, $\pi/2+\arctan(\eta/L)\sim-L/\eta$, giving $I\sim1/(1-\gamma)$. For $\eta\to+\infty$ it tends to $\pi$, giving $I\sim\pi/(\varepsilon\log2)$, the $\gamma\downarrow1$ limit of the interior-peak approximation. These are [overlap regions](../../../../../../../overlap-region.md) with $\varepsilon\ll|\gamma-1|\ll1$, not assertions that the fixed-$\eta$ remainder is uniform to arbitrarily large $\eta$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
