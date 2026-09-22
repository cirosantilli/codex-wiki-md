<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [voltage](../../../../../voltage.md) [nullcline](../../../../../nullcline.md) is $g(v,n)=I^*$ and the recovery [nullcline](../../../../../nullcline.md) is $n=n_\infty(v)$. In the relevant region $g_n>0$, so below the [voltage](../../../../../voltage.md) curve $\dot v>0$ and above it $\dot v<0$. Below the recovery curve $\dot n>0$, while above it $\dot n<0$.

For small $\epsilon$, the outer [voltage](../../../../../voltage.md) branches with $g_v>0$ attract fast [voltage](../../../../../voltage.md) motion; the middle branch with $g_v<0$ repels it. Arrange the intersections so the equilibrium is on that middle branch, with recovery increasing along the high-[voltage](../../../../../voltage.md) attracting branch and decreasing along the low-[voltage](../../../../../voltage.md) attracting branch. The trajectory then drifts towards a fold, jumps rapidly to the other attracting branch at nearly constant $n$, and repeats. This is a [relaxation oscillation](../../../../../relaxation-oscillation.md).

The local [linear stability](../../../../../linear-stability.md) calculation supports the construction. At an equilibrium,

$$
J=\begin{pmatrix}-g_v/\epsilon&-g_n/\epsilon\\n_\infty'&-1\end{pmatrix},\qquad\operatorname{tr}J=-g_v/\epsilon-1,\qquad\det J=\frac{g_v+g_nn_\infty'}{\epsilon}.
$$

A sufficiently steep recovery curve gives positive determinant, while $g_v<-\epsilon$ gives positive trace. Hence the equilibrium is a repeller. The bounded physical rectangle can be chosen forward invariant, and a small neighborhood of the repeller removed to give a trapping annulus. The [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) then supplies a [periodic orbit](../../../../../periodic-orbit.md). These conditions can be realized because the recovery function and the applied current control the intersection and its slope; oscillation is possible, not forced for every choice.

For the illustration, $\gamma_K=0.1$, $H=0.8$, $v_K=0.2$, $\epsilon=0.01$, $I^*=0$, $M(v)=(1+e^{-25(v-0.2)})^{-1}$ and $n_\infty(v)=0.8/(1+e^{-20v})$. The rectangle $[-0.2,1]\times[0,0.8]$ has inward-pointing flow, and the displayed numerical trajectory realizes the folded-branch mechanism.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematical physiology course of the University of Oxford](../../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
