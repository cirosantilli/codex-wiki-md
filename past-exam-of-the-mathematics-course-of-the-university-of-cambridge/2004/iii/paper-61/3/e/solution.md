<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

To first order in the potential, $a=A=1+O(q^2)$, while the spatial and temporal [Volterra integral equations](../../../../../../volterra-integral-equation.md) give

$$
b(k)=-\int_0^\infty e^{2ikx}q_0(x)dx+O(q^3),\qquad B(k)=-\int_0^T e^{4ik^2s}\bigl[2k g_0(s)+ig_1(s)\bigr]ds+O(q^3).
$$

Thus the linear limit of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) is exactly

$$
\widehat q_0(-2k)-e^{4ik^2T}\widehat q(-2k,T)=\int_0^T e^{4ik^2s}\bigl[2k g_0(s)+ig_1(s)\bigr]ds,
$$

for the linear equation $iq_t+q_{xx}=0$. This ties the two boundary traces together, rather than allowing them to be independent data.

The count is made explicit by a temporal [Laplace transform](../../../../../../laplace-transform.md). For $\operatorname{Re}p>0$, the transformed equation is $\widetilde q_{xx}+ip\widetilde q=iq_0$. Put $\alpha=\sqrt{-ip}$ with positive real part. Of the two homogeneous solutions $e^{\pm\alpha x}$, only $e^{-\alpha x}$ decays at infinity. There is therefore exactly one free complex coefficient to be fixed at the endpoint. In particular, prescribed Dirichlet trace $\widetilde g_0$ gives the definite Neumann trace

$$
\widetilde g_1(p)=-\alpha\widetilde g_0(p)-i\int_0^\infty e^{-\alpha y}q_0(y)dy.
$$

This follows by differentiating the decaying Dirichlet Green kernel $-(e^{-\alpha|x-y|}-e^{-\alpha(x+y)})/(2\alpha)$ at $x=0$. Thus **one complex boundary condition is needed**, such as Dirichlet, Neumann or a suitable Robin combination. Prescribing both traces arbitrarily would overdetermine the problem. In a [Sobolev space](../../../../../../sobolev-space-split.md) with the required trace regularity, the cubic term is a locally Lipschitz perturbation, so the small-data perturbative problem retains the same boundary-condition count; corner compatibility still must be imposed for a classical solution.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
