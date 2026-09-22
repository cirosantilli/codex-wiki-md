<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md) and [rotational symmetry](../../../../../../rotational-symmetry.md), including [reflection in mathematics](../../../../../../reflection-mathematics.md) invariance of the spherical geometry, determine the possible rigid motions before any calculation. Translation is a [polar vector](../../../../../../polar-vector.md); its linear dependence on a single [vector](../../../../../../vector.md) $\mathbf A$ must be $c\mathbf A$. A [traceless second-rank tensor](../../../../../../traceless-second-rank-tensor.md) $\mathbf B$ cannot produce a polar [vector](../../../../../../vector.md) by an isotropic linear map: [tensor contraction](../../../../../../tensor-contraction.md) with the [identity matrix](../../../../../../identity-matrix.md) vanishes and [tensor contraction](../../../../../../tensor-contraction.md) with the [totally antisymmetric tensor](../../../../../../totally-antisymmetric-tensor.md) vanishes because $\mathbf B$ is a [symmetric second-rank tensor](../../../../../../symmetric-second-rank-tensor.md). [Angular velocity](../../../../../../angular-velocity.md) is an [axial vector](../../../../../../pseudovector.md). Neither $\mathbf A$ nor a symmetric $\mathbf B$ can produce one by an isotropic linear map. Products such as $\mathbf A\times\mathbf B\mathbf A$ are excluded by [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md). Thus $\boldsymbol\Omega=0$.

Use the [Unscaled Papkovich–Neuber representation](../../../../../../unscaled-papkovich-neuber-representation.md), with [harmonic functions](../../../../../../harmonic-function.md) $\boldsymbol\Phi$ and $\chi$:

$$
\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,
\qquad p-p_\infty=2\mu\nabla\cdot\boldsymbol\Phi.
$$

Indeed $\nabla\cdot\mathbf u=0$ and $\mu\nabla^2\mathbf u=\nabla p$ because each potential is a [harmonic function](../../../../../../harmonic-function.md). Put $r=|\mathbf x|$ and $S=\mathbf x\cdot\mathbf B\mathbf x$. The decaying [harmonic functions](../../../../../../harmonic-function.md) with the necessary angular dependence are $\mathbf A\cdot\mathbf x/r^3$, $\mathbf B\mathbf x/r^3$ and $S/r^5$. The last is a [harmonic function](../../../../../../harmonic-function.md) precisely because $\operatorname{tr}\mathbf B=0$. A $1/r$ [Stokeslet](../../../../../../stokeslet.md) is excluded by the [force-free](../../../../../../force-free.md) condition, and a [rotlet](../../../../../../rotlet.md) by the [torque-free](../../../../../../torque-free.md) condition. Try

$$
\boldsymbol\Phi=d\frac{\mathbf B\mathbf x}{r^3},\qquad
\chi=c\frac{\mathbf A\cdot\mathbf x}{r^3}+e\frac{S}{r^5}.
$$

The resulting [Stokes flow](../../../../../../stokes-flow-split.md) is

$$
\mathbf u=c\left(\frac{\mathbf A}{r^3}-\frac{3(\mathbf A\cdot\mathbf x)\mathbf x}{r^5}\right)
-3d\frac{S\mathbf x}{r^5}
+e\left(\frac{2\mathbf B\mathbf x}{r^5}-\frac{5S\mathbf x}{r^7}\right).
$$

At $r=a$, the coefficient of $\mathbf n(\mathbf A\cdot\mathbf n)$ fixes $c=a^3/3$; the remaining constant [vector](../../../../../../vector.md) gives $\mathbf U=-2\mathbf A/3$. In the $\mathbf B$ mode, matching $\mathbf B\mathbf n-(\mathbf n\cdot\mathbf B\mathbf n)\mathbf n$ gives $e=a^4/2$ and $d=-a^2/2$. Therefore the complete [two-mode tensorial squirmer flow](../../../../../../two-mode-tensorial-squirmer-flow.md) is

$$
\boxed{\begin{aligned}
\mathbf u(\mathbf x)&=\frac{a^3}{3r^3}\left[\mathbf A-3(\mathbf A\cdot\widehat{\mathbf x})\widehat{\mathbf x}\right]
\\&\quad+\frac{3a^2 S\mathbf x}{2r^5}
+\frac{a^4}{2}\left(\frac{2\mathbf B\mathbf x}{r^5}-\frac{5S\mathbf x}{r^7}\right),\\
p-p_\infty&=3\mu a^2\frac{S}{r^5},\qquad
\mathbf U=-\frac23\mathbf A,\quad\boldsymbol\Omega=0.
\end{aligned}}
$$

The [boundary condition](../../../../../../boundary-condition.md) is satisfied in the laboratory frame, so the [Stokes flow](../../../../../../stokes-flow-split.md) tends to zero at infinity. The [potential dipole](../../../../../../potential-dipole.md) in the $\mathbf A$ mode gives an [irrotational flow](../../../../../../irrotational-flow.md) and decays as $r^{-3}$; the leading $\mathbf B$ mode is a [stresslet](../../../../../../force-dipole-flow.md), decaying as $r^{-2}$. Neither carries a net [force](../../../../../../force.md) or [torque](../../../../../../torque.md). Direct [surface integral](../../../../../../surface-integral.md) averaging with the [surface slip velocity](../../../../../../surface-slip-velocity.md) formula gives the same translation, providing an independent check. [Uniqueness of Stokes flow](../../../../../../uniqueness-of-stokes-flow.md) then identifies this decaying solution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
