<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real locally integrable function, the definitions are distributional:

$$
\boxed{\begin{aligned}f\text{ subharmonic}&\iff\int_\Omega f\Delta\phi\geq0\quad(0\leq\phi\in C_c^\infty(\Omega)),\\
f\text{ superharmonic}&\iff\int_\Omega f\Delta\phi\leq0\quad(0\leq\phi\in C_c^\infty(\Omega)),\\
f\text{ harmonic}&\iff\int_\Omega f\Delta\phi=0\quad(\phi\in C_c^\infty(\Omega)).\end{aligned}}
$$

Thus the [Laplacian](../../../../../../laplacian.md) is respectively a [positive distribution](../../../../../../positive-distribution.md), a negative distribution, or zero. A [superharmonic function](../../../../../../superharmonic-function.md) is the negative of a [subharmonic function](../../../../../../subharmonic-function.md); being both is equivalent to being harmonic. For a $C^2$ function these conditions are $\Delta f\geq0$, $\Delta f\leq0$, and $\Delta f=0$ pointwise.

An $L^1_{\mathrm{loc}}$ equivalence class does not itself specify point values. For the maximum principle use the [canonical representative of a subharmonic distribution](../../../../../../canonical-representative-of-a-subharmonic-distribution.md)

$$
\widetilde f(x)=\lim_{r\downarrow0}\frac1{|B_r|}\int_{B_r(x)}f.
$$

These normalized integrals are ball averages. To justify this construction, first mollify $f$: its smooth local regularizations satisfy $\Delta f_\varepsilon\geq0$. For any smooth subharmonic function, the spherical mean $m_x(r)$ obeys

$$
m_x'(r)=\frac1{|\mathbb S^{n-1}|r^{n-1}}\int_{B_r(x)}\Delta f\geq0.
$$

This follows by differentiating the spherical integral and applying the [divergence theorem](../../../../../../divergence-theorem.md). Its ball mean also increases with radius: its derivative is $n/r$ times the spherical mean minus the ball mean. Local $L^1$ convergence of the regularizations passes the monotonicity of the ball means to $f$. The decreasing-radius limit therefore exists, possibly as minus infinity at an exceptional point, and equals $f$ almost everywhere by the [Lebesgue differentiation theorem](../../../../../../lebesgue-differentiation-theorem.md). It is [upper semicontinuous](../../../../../../upper-semicontinuity.md) as the local infimum of continuous ball averages and satisfies

$$
\widetilde f(x)\leq\frac1{|B_r|}\int_{B_r(x)}\widetilde f.
$$

For a [superharmonic function](../../../../../../superharmonic-function.md) use the corresponding [lower semicontinuous](../../../../../../lower-semicontinuity.md) representative and reverse the inequality.

For a distributionally [harmonic function](../../../../../../harmonic-function.md), the smooth regularizations are harmonic and have constant spherical means. A radial [mollifier](../../../../../../mollifier.md) $\rho_\delta$ of integral one therefore reproduces them by averaging these means. At fixed interior radius $\delta$, pass to the local $L^1$ limit to obtain $f=f*\rho_\delta$ almost everywhere on a smaller region. The right side is smooth and has zero distributional Laplacian, giving the smooth harmonic representative. This proves the relevant [Weyl lemma](../../../../../../weyl-lemma.md). Changing a value at a single point can spoil a pointwise maximum principle, so the representative convention is essential.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
