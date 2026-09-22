<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The squared [norm](../../../../../norm.md) of $p_\ell(x)e^{-x^2/4}$ in $L^2(\mathbb R,dx)$ is $\sqrt{2\pi}\,h_\ell$, where $(h_0,h_1,h_2)=(1,1,2)$. Choose positive normalizing constants

$$
\boxed{\kappa_0=\kappa_1=(2\pi)^{1/4},\qquad
\kappa_2=\sqrt2(2\pi)^{1/4}.}
$$

Then $\phi_0,\phi_1,\phi_2$ are an [orthonormal set](../../../../../orthonormal-set.md) for [Lebesgue measure](../../../../../lebesgue-measure.md). Expanding the finite sums gives

$$
\begin{aligned}
\int\widetilde K_3(x,y)\widetilde K_3(y,z)\,dy
&=\sum_{\ell,m=0}^2\phi_\ell(x)\phi_m(z)
\int\phi_\ell(y)\phi_m(y)\,dy\\
&=\sum_{\ell=0}^2\phi_\ell(x)\phi_\ell(z)
=\widetilde K_3(x,z).
\end{aligned}
$$

Thus this is an [orthogonal polynomial projection kernel](../../../../../orthogonal-polynomial-projection-kernel.md), explicitly

$$
\boxed{\widetilde K_3(x,y)
=\frac{e^{-(x^2+y^2)/4}}{\sqrt{2\pi}}
\left[1+xy+\frac{(x^2-1)(y^2-1)}2\right].}
$$

The positive constants above are forced by the reproducing identity: before normalization, its convolution multiplies each independent term $\phi_\ell(x)\phi_\ell(z)$ by $\sqrt{2\pi}h_\ell/\kappa_\ell^2$. Each multiplier must equal one. Changing the sign of a real $\kappa_\ell$ leaves the kernel unchanged.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
