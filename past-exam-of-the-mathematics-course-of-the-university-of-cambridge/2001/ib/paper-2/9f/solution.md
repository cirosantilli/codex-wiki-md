<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

For $H=p^2/(2m)+V(x)$ and a time-independent operator $O$, differentiate its [expectation value](../../../../../expectation-value.md) and use the [Schrödinger equation](../../../../../schrodinger-equation.md) and its adjoint. Moving $H$ across the inner product by integration by parts gives

$$
\frac{d}{dt}\langle O\rangle=\frac{i}{\hbar}\langle HO-OH\rangle=\frac{i}{\hbar}\langle[H,O]\rangle.
$$

Work with wavefunctions in the displayed operators' domains; the vanishing at infinity removes the associated boundary terms. This is the [Ehrenfest theorem](../../../../../ehrenfest-theorem.md) derived from time evolution.

The [canonical commutation relation](../../../../../canonical-commutation-relation.md) follows directly from differentiating $x\psi$: $[p,x]\psi=-i\hbar\psi$. Thus $[p^2,x]=p[p,x]+[p,x]p=-2i\hbar p$, while $[V(x),x]=0$. It follows that

$$
\boxed{\frac{d}{dt}\langle x\rangle=\frac{\langle p\rangle}{m}.}
$$

For the momentum equation, apply both products to a test wavefunction:

$$
[V,p]\psi=-i\hbar V\psi'+i\hbar(V\psi)'=i\hbar V'\psi.
$$

The kinetic term commutes with $p$, so $[H,p]=i\hbar V'$. Therefore

$$
\boxed{\frac{d}{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

These are the [classical equations from Ehrenfest theorem](../../../../../classical-equations-from-ehrenfest-theorem.md) for position and momentum expectations; the force expectation need not equal the force evaluated at the expected position.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
