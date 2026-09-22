<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d(\mathbf y,t)=[u^{[n]}]$ denote the signed opening, positive when the faces separate, and let $S$ be the crack surface. Its displacement jump is $\mathbf b=d\mathbf n$. The singular strain associated with this jump has moment density $c_{ijkl}b_kn_l$. For the isotropic [elastic stiffness tensor](../../../../../../elastic-stiffness-tensor.md), contraction gives

$$
m_{ij}(\mathbf y,t)=d(\mathbf y,t)\left[\lambda\delta_{ij}+2\mu n_i(\mathbf y)n_j(\mathbf y)\right].
$$

The equivalent distributional [body force](../../../../../../body-force.md) is the negative divergence of this prescribed moment density:

$$
\boxed{f_i(\mathbf x,t)=-\partial_{x_j}\int_S
 d(\mathbf y,t)[\lambda\delta_{ij}+2\mu n_i(\mathbf y)n_j(\mathbf y)]
 \delta^{(3)}(\mathbf x-\mathbf y)\,dS_{\mathbf y}}.
$$

The resulting forced [elastic wave in an isotropic solid](../../../../../../elastic-wave-in-an-isotropic-solid.md) equation is $\rho u_{i,tt}=\partial_j\sigma_{ij}+f_i$. This is a [tensile-crack seismic source](../../../../../../tensile-crack-seismic-source.md); it need not be represented as an ordinary smooth volume force. For a small nearly planar patch of area $S_0$, uniform normal $\mathbf n$ and opening $d(t)$, define its volume change $V(t)=S_0d(t)$. Its [seismic moment tensor](../../../../../../seismic-moment-tensor.md) and point-source force are

$$
\boxed{M_{ij}(t)=V(t)(\lambda\delta_{ij}+2\mu n_in_j),\qquad
f_i=-M_{ij}(t)\partial_{x_j}\delta^{(3)}(\mathbf x-\mathbf y_0)}.
$$

The sign convention makes a positive opening a positive extensional moment. Reversing the convention for the displacement jump changes both signs together; the force is independent of reversing the orientation of the crack normal.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
