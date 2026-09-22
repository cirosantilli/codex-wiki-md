<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The $k_0^2uv$ terms cancel in $uL_Hv-vL_Hu$. For a ball $B_R$, the [product rule](../../../../product-rule.md) and [divergence theorem](../../../../divergence-theorem.md) give [Green's second identity](../../../../green-second-identity.md) in the form

$$
\int_{B_R}(uL_Hv-vL_Hu)\,d^3r=\int_{\partial B_R}(u\partial_nv-v\partial_nu)\,dS.
$$

Thus the whole-space integral vanishes when this boundary term tends to zero. For example, uniform bounds $u,v=O(R^{-1-\epsilon})$ and $\nabla u,\nabla v=O(R^{-1-\epsilon})$, with $\epsilon>0$, make it $O(R^{-2\epsilon})$.

**Pointwise vanishing alone, as stated in the source, is insufficient.** Smooth fields agreeing with $u=\sin(k_0r)/r$ and $v=\cos(k_0r)/r$ outside a ball both tend to zero, but their distant boundary integral is $-4\pi k_0$. One may smooth them inside the ball without changing that flux. The requested zero identity therefore needs sufficient decay or boundary/radiation conditions that actually eliminate the boundary term.

For the generalized [plane wave](../../../../plane-wave.md) eigenfunctions, their [orthogonality](../../../../orthogonal-vectors.md) is distributional:

$$
\begin{aligned}
\int_{\mathbb R^3}\psi_{k_1}^*(r)\psi_{k_2}(r)d^3r
&=\frac1{(2\pi)^3}\prod_{j=1}^3\int_{\mathbb R}e^{i(k_{2j}-k_{1j})r_j}dr_j\\
&=\prod_{j=1}^3\delta(k_{2j}-k_{1j})=\delta^{(3)}(k_1-k_2).
\end{aligned}
$$

Here $\int e^{iqx}dx=2\pi\delta(q)$ is the [Fourier representation of the Dirac delta function](../../../../fourier-representation-of-the-dirac-delta-function.md). These eigenfunctions are not ordinary square-integrable functions or decaying test fields.

Expand $\Phi=\int A_k\psi_k\,d^3k$ and define $V_k=\int\psi_k^*(r')V(r')d^3r'$. Since $L_H\psi_k=(k_0^2-k^2)\psi_k$, projection of the source equation gives $(k_0^2-k^2)A_k=V_k$. Formally dividing and substituting back gives

$$
\boxed{\Phi(r)=\frac1{(2\pi)^3}\int_{\mathbb R^3}d^3k\int_{\mathbb R^3}d^3r'\,\frac{e^{ik\cdot(r-r')}}{k_0^2-k^2}V(r').}
$$

At the shell $k=k_0$, a pole prescription is required; homogeneous solutions can otherwise be added. The formula is an inverse of the [Helmholtz equation](../../../../helmholtz-equation.md) with that convention still to be selected.

Let $H$ denote the kernel in this source formula, so $L_HH=+\delta^{(3)}$. Put $l=|r-r'|$ and align the Fourier polar axis with $r-r'$. Angular integration gives

$$
\int_{S^2}e^{ikl\cos\theta}d\Omega=2\pi\int_{-1}^1e^{ikl\mu}d\mu=4\pi\frac{\sin(kl)}{kl}.
$$

Consequently the [radial Fourier representation of the Helmholtz Green function](../../../../radial-fourier-representation-of-the-helmholtz-green-function.md) gives

$$
H(l)=\frac1{2\pi^2l}\int_0^\infty\frac{k\sin(kl)}{k_0^2-k^2}dk.
$$

The last Green function written in the PDF has the opposite denominator. It is obtained by setting $G=-H$, the common convention $L_HG=-\delta^{(3)}$:

$$
\boxed{G(l)=\frac1{2\pi^2l}\int_0^\infty\frac{k\sin(kl)}{k^2-k_0^2}dk,\qquad\Phi(r)=-\int G(r,r')V(r')d^3r'.}
$$

Thus the two displayed source and Green formulas are consistent only when this minus sign is retained; $G$ cannot also be the positive-delta inverse kernel.

Finally the integral is not an ordinary improper integral across $k=k_0$. A [Cauchy principal value](../../../../cauchy-principal-value.md) yields $G_{\rm PV}(l)=\cos(k_0l)/(4\pi l)$. The outgoing prescription $k^2-k_0^2-i0$ yields the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md), $G_+(l)=e^{ik_0l}/(4\pi l)$; the opposite sign gives the incoming wave. The [Sokhotski–Plemelj formula](../../../../sokhotski-plemelj-theorem.md) accounts for their difference. The source does not specify which prescription is intended, so the boxed radial expression must be read with one chosen consistently.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
