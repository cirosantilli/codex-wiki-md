<h1 id="34a/solution">Solution</h1>

↑ **Parent:** [34A](../34a.md)

For part (a), the [adjoint operator](../../../../../adjoint-operator.md) is

$$
A^\dagger=\frac{m\omega X-iP}{\sqrt{2m\hbar\omega}}.
$$

Using the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[X,P]=i\hbar I$,

$$
[A,A^\dagger]
=\frac1{2m\hbar\omega}[m\omega X+iP,m\omega X-iP]
=\boxed{I}.
$$

Thus $A$ and $A^\dagger$ are the [annihilation and creation operators](../../../../../creation-and-annihilation-operators.md) of the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md).

For part (b), write

$$
K=\frac12(A^{\dagger2}-A^2),
\qquad S(\gamma)=e^{-\gamma K}.
$$

Since $[A,K]=A^\dagger$ and $[A^\dagger,K]=A$, differentiation of the [unitary conjugation](../../../../../unitary-conjugation.md) gives

$$
\frac d{d\gamma}A(\gamma)
=-S^\dagger[A,K]S=-A^\dagger(\gamma),
\qquad
\frac d{d\gamma}A^\dagger(\gamma)=-A(\gamma).
$$

The initial conditions are $A(0)=A$ and $A^\dagger(0)=A^\dagger$. Solving this pair of [linear ordinary differential equations](../../../../../linear-ordinary-differential-equation.md) gives the [Bogoliubov transformation](../../../../../bogoliubov-transformation.md)

$$
\boxed{A(\gamma)=A\cosh\gamma-A^\dagger\sinh\gamma.}
$$

This is the transformation implemented by the [single-mode squeeze operator](../../../../../single-mode-squeeze-operator.md).

For part (c), invert the definition of $A$:

$$
X=\sqrt{\frac{\hbar}{2m\omega}}(A+A^\dagger),
\qquad
P=-i\sqrt{\frac{m\hbar\omega}{2}}(A-A^\dagger).
$$

The transformation above implies

$$
S^\dagger XS=e^{-\gamma}X,
\qquad
S^\dagger PS=e^\gamma P.
$$

The [ground state](../../../../../ground-state.md) has zero position and momentum means and variances $\hbar/(2m\omega)$ and $m\hbar\omega/2$. Hence the [squeezed vacuum state](../../../../../squeezed-vacuum-state.md) $|\gamma\rangle=S(\gamma)|0\rangle$ has

$$
(\Delta X)^2_\gamma=e^{-2\gamma}\frac{\hbar}{2m\omega},
\qquad
(\Delta P)^2_\gamma=e^{2\gamma}\frac{m\hbar\omega}{2}.
$$

The reciprocal squeezing factors cancel, so

$$
\boxed{\Delta X\,\Delta P=\frac\hbar2.}
$$

The state therefore continues to saturate the [Heisenberg uncertainty relation](../../../../../robertson-uncertainty-principle.md).

## ↑ Ancestors (10)

1. [34A](../34a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
