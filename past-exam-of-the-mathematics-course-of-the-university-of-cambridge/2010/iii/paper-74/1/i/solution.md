<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Adding $i$ times the equation for $B$ to the equation for $A$ combines the two real amplitudes into $P=A+iB$. With the fluctuating coupling absent, the derivative terms satisfy $-rB_x+irA_x=irP_x$, so the complex evolution is

$$
P_t=\mathcal L_rP,\qquad \mathcal L_r=\partial_x^2+ir\partial_x-1.
$$

Both real amplitudes satisfy the zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), hence $P(0)=P(\ell)=0$. A unit-modulus change of dependent variable removes the first derivative: put $P=e^{-irx/2}F$. Direct differentiation gives

$$
\mathcal L_rP=e^{-irx/2}\left[F''+\left(\frac{r^2}{4}-1\right)F\right].
$$

The [eigenfunctions](../../../../../../eigenfunction.md) satisfying the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) are therefore $e^{-irx/2}\sin(n\pi x/\ell)$, with temporal [eigenvalues](../../../../../../eigenvalue.md)

$$
\sigma_n=\frac{r^2}{4}-1-\frac{n^2\pi^2}{\ell^2},\qquad n=1,2,\ldots.
$$

The first nonzero stationary mode appears when $\sigma_1=0$, giving

$$
\boxed{r_0=2\sqrt{1+\pi^2/\ell^2},\qquad P_0=C e^{-ir_0x/2}\sin(\pi x/\ell).}
$$

The complex constant $C$ supplies the phase freedom of this unperturbed [mean-field dynamo](../../../../../../mean-field-dynamo.md) model.

To display the [dipole and quadrupole parity in a mean-field dynamo](../../../../../../dipole-and-quadrupole-parity-in-a-mean-field-dynamo.md), center the coordinate at the midpoint: $y=x-\ell/2$, $F(y)=\cos(\pi y/\ell)$, $h=r_0/2$. Choose a real amplitude $C_0$. The dipole choice is $P_D=C_0F(y)e^{-ihy}$, so

$$
\boxed{A_D=C_0\cos(\pi y/\ell)\cos(hy),\qquad B_D=-C_0\cos(\pi y/\ell)\sin(hy).}
$$

Here $A_D$ is an [even function](../../../../../../even-function.md) and $B_D$ an [odd function](../../../../../../odd-function.md) of $y$, and the cosine envelope vanishes at both boundaries. The quadrupole choice is $P_Q=iP_D$, which gives

$$
\boxed{A_Q=C_0\cos(\pi y/\ell)\sin(hy),\qquad B_Q=C_0\cos(\pi y/\ell)\cos(hy).}
$$

Now $A_Q$ is an [odd function](../../../../../../odd-function.md) and $B_Q$ an [even function](../../../../../../even-function.md). Both choices have the same stationary threshold because the unperturbed complex equation is invariant under a constant phase rotation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
