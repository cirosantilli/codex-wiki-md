<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\lambda>0$, the [scalar potential](../../../../scalar-potential.md) is minimized at $\phi^\dagger\phi=v^2/2$. With the specified upper-component [vacuum expectation value](../../../../vacuum-expectation-value.md) $\phi_0=(v,0)^T/\sqrt2$ and [hypercharge](../../../../hypercharge.md) $Y=-I/2$, the unbroken generator is

$$
Q=T^3+Y=\begin{pmatrix}0&0\\0&-1\end{pmatrix},\qquad Q\phi_0=0.
$$

The other three independent generator directions act nontrivially on $\phi_0$. Thus the connected unbroken gauge subgroup is $U(1)_{\rm em}$, while three gauge directions are broken. The [normalization](../../../../normalization.md) here is $Q=T^3+Y$, not the alternative convention in which [hypercharge](../../../../hypercharge.md) is doubled.

Apply the [covariant derivative](../../../../covariant-derivative.md) directly to the vacuum:

$$
D_\mu\phi_0=-\frac{iv}{2\sqrt2}
\begin{pmatrix}g_2A_\mu^3-g_1B_\mu\\g_2(A_\mu^1+iA_\mu^2)\end{pmatrix}.
$$

In the mostly-plus convention the canonical [scalar](../../../../scalar.md) kinetic term is $-(D_\mu\phi)^\dagger D^\mu\phi$. Its quadratic vector terms are

$$
\mathcal L_{\rm mass}=-\frac{v^2}{8}
\left[g_2^2(A_\mu^1A^{1\mu}+A_\mu^2A^{2\mu})
+(g_2A_\mu^3-g_1B_\mu)(g_2A^{3\mu}-g_1B^\mu)\right].
$$

Define $s_W=\sin\theta_W=g_1/\sqrt{g_1^2+g_2^2}$ and $c_W=\cos\theta_W=g_2/\sqrt{g_1^2+g_2^2}$. Diagonalization gives

$$
\boxed{W_\mu^\pm=\frac{A_\mu^1\mp iA_\mu^2}{\sqrt2},\qquad
Z_\mu=c_WA_\mu^3-s_WB_\mu,\qquad
A_\mu^\gamma=s_WA_\mu^3+c_WB_\mu.}
$$

The neutral combination $Z$ lies along the nonzero [eigenvector](../../../../eigenvector.md) $(g_2,-g_1)$; the orthogonal combination $(g_1,g_2)$ is the massless [photon](../../../../photon.md). Comparing the [mass](../../../../mass.md) terms with $-m_W^2W^+\cdot W^--m_Z^2Z^2/2$ yields

$$
\boxed{m_W=\frac{g_2v}{2},\qquad
m_Z=\frac v2\sqrt{g_1^2+g_2^2},\qquad
m_\gamma=0,\qquad\frac{m_W}{m_Z}=\cos\theta_W.}
$$

Finally insert the inverse neutral rotation into the coupling:

$$
g_2T^3A_\mu^3+g_1YB_\mu
=(g_2s_WT^3+g_1c_WY)A_\mu^\gamma
+(g_2c_WT^3-g_1s_WY)Z_\mu.
$$

Both coefficients in the [photon](../../../../photon.md) term agree, giving

$$
\boxed{e=g_2\sin\theta_W=g_1\cos\theta_W
=\frac{g_1g_2}{\sqrt{g_1^2+g_2^2}},\qquad D_\mu\supset-ieQA_\mu^\gamma.}
$$

The upper vacuum component is electrically neutral and the lower [scalar](../../../../scalar.md) component has charge $-e$, consistently with the source's negative [hypercharge](../../../../hypercharge.md). This doublet is the conjugate convention to the commonly displayed positive-hypercharge doublet; it does not change the vector masses or the electromagnetic coupling. The four real [scalar](../../../../scalar.md) components supply three would-be [Goldstone modes](../../../../goldstone-boson.md) and one physical radial Higgs mode, preserving the total physical degrees of freedom.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
