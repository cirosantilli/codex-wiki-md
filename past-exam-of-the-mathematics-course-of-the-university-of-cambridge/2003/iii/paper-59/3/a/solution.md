<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take small incoming sections $y=\pm h$ and outgoing sections $x=\pm h$ after straightening the [stable manifold](../../../../../../stable-manifold.md) and [unstable manifold](../../../../../../unstable-manifold.md) of the origin. Its [eigenvalues](../../../../../../eigenvalue.md) are $1,-\delta$, so the leading local passage satisfies $x(t)=x_0e^t$, $y(t)=y_0e^{-\delta t}$. The exit time and transverse exit coordinate are

$$
T=\log\frac{h}{|x_0|},\qquad y_{\mathrm{out}}=\operatorname{sgn}(y_0)h^{1-\delta}|x_0|^\delta.
$$

Thus the local passage contracts strongly as $x_0\to0$, while its duration diverges. Smooth global reinjection from the right outgoing section to the upper incoming section has leading transverse coordinate $-\mu+K_Ry_{\mathrm{out}}$; the corresponding left-to-lower return has $\nu+K_Ly_{\mathrm{out}}$. Choose the parameters as these signed splitting coordinates and absorb $h^{1-\delta}$ into $A,B$.

After scaling the incoming-section labels to $y_n=\pm1$, the leading [Poincaré return map](../../../../../../poincare-map.md) is

$$
x_{n+1}=\begin{cases}-\mu+A\operatorname{sgn}(y_n)|x_n|^\delta,&x_n>0,\\
\nu+B\operatorname{sgn}(y_n)|x_n|^\delta,&x_n<0,
\end{cases}\qquad y_{n+1}=\operatorname{sgn}(x_n).
$$

The second coordinate records which outgoing branch was used, not an independent continuous amplitude. A smooth planar flow preserves the orientation of a transverse-section return. For the right-to-upper pair of sections, the ordered pair consisting of the flow direction and the positive section tangent has the same orientation at both ends; the same is true for the left-to-lower pair. Hence $A,B>0$ for these sign conventions and a nondegenerate global return.

For general nonlinear $P,Q$, this is an **asymptotic return model**, with smooth parameter corrections and higher-order local-passage corrections. The hypotheses do not imply an exact power-law map in the original coordinates. Interpreting the printed parameters themselves as linear splitting coordinates also requires a nondegenerate two-parameter unfolding: the two splitting derivatives must be nonzero. For example, composing a generic right-loop splitting with $\mu\mapsto\mu^2$ preserves the stated loop at $\mu=0$ but does not give the printed signed $-\mu$ offset. The subsequent region diagram uses the standard generic splitting-coordinate interpretation. Nor is $x=0$ a normal return point: it lies on the [stable manifold](../../../../../../stable-manifold.md), whose trajectory takes infinite time to reach the [saddle equilibrium](../../../../../../saddle-equilibrium.md). This explains how the map describes nearby recurrent trajectories without extending a finite-time return across the singular separatrix.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
