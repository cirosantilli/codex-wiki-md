<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First use the actual PDF boost bracket $[K_i,K_j]=-i\epsilon_{ijk}J_k$; replacing the final $J_k$ by $K_k$, as the TeX transcription does, would be a different and incorrect algebra. Expanding the three brackets yields

$$
\begin{aligned}
[A_i,A_j]&=\tfrac14([J_i,J_j]+i[J_i,K_j]+i[K_i,J_j]-[K_i,K_j])
=i\epsilon_{ijk}A_k,\\
[B_i,B_j]&=i\epsilon_{ijk}B_k,\\
[A_i,B_j]&=\tfrac14([J_i,J_j]-i[J_i,K_j]+i[K_i,J_j]+[K_i,K_j])=0.
\end{aligned}
$$

Thus

$$
\boxed{\mathfrak{so}(1,3)_{\mathbb C}
\cong\mathfrak{sl}_2(\mathbb C)\oplus\mathfrak{sl}_2(\mathbb C),
\qquad\mathbf J=\mathbf A+\mathbf B.}
$$

The two sets have SU(2)-type brackets. Their compact real form exponentiates to $SU(2)\times SU(2)$, whereas their full complexification exponentiates to $SL(2,\mathbb C)\times SL(2,\mathbb C)$. This does not turn the physical real [Lorentz group](../../../../../lorentz-group.md) into a compact product. With Hermitian $J,K$, $A^\dagger=B$, and the two factors are tied by the Lorentz reality condition; the connected physical [spin](../../../../../spin.md) cover is $SL(2,\mathbb C)$.

For the right-handed spinor representation, the supplied sigma formula gives $\bar\sigma^{ij}=\epsilon_{ijk}\sigma_k/2$ and $\bar\sigma^{0i}=i\sigma_i/2$. Therefore

$$
\boxed{J_i=\frac{\sigma_i}{2},\qquad K_i=\frac{i\sigma_i}{2},
\qquad A_i=0,\quad B_i=\frac{\sigma_i}{2}.}
$$

It is the $(0,1/2)$ representation in this definition of $A,B$. These are finite-dimensional representation matrices; the boosts are not Hermitian for a positive-definite spinor inner product, as expected for a noncompact group. They are distinct from the operator-component [commutator](../../../../../commutator.md) coefficients discussed in Question 1.

For the group map, encode a real Minkowski vector by the Hermitian matrix

$$
X=x_\mu\sigma^\mu=x^\nu\sigma_\nu,
\qquad\det X=(x^0)^2-|\mathbf x|^2.
$$

The trace identity $\tfrac12\operatorname{Tr}(\bar\sigma^\mu\sigma_\nu)=\delta^\mu{}_{\nu}$ recovers its contravariant components. For $N\in SL(2,\mathbb C)$, $X'=NXN^\dagger$ is Hermitian and has the same determinant. Expanding $X'$ in that basis gives

$$
\boxed{x'^\mu=\Lambda^\mu{}_{\nu}(N)x^\nu,
\qquad\Lambda^\mu{}_{\nu}(N)
=\frac12\operatorname{Tr}(\bar\sigma^\mu N\sigma_\nu N^\dagger).}
$$

The coefficients are real because the trace of a product of Hermitian matrices is real. Equality of determinants for all $x$ proves $\Lambda^T\eta\Lambda=\eta$. The action for $N_1N_2$ is the composition of the two actions, proving the homomorphism law.

Since $SL(2,\mathbb C)$ is connected and the identity maps to the identity, its image has determinant $+1$ and preserves time orientation. More directly, positive-definite matrices representing future timelike vectors remain positive definite under $X\mapsto NXN^\dagger$. The kernel is $\{I,-I\}$: if every Hermitian $X$ is fixed, $X=I$ first makes $N$ unitary, and then commutation with all Hermitian matrices makes it a scalar with determinant one.

Conversely, $SU(2)$ gives every spatial rotation, and positive Hermitian determinant-one matrices $\exp(\mathbf b\cdot\boldsymbol\sigma/2)$ give every pure boost. Rotation-boost decomposition yields every proper orthochronous [Lorentz transformation](../../../../../lorentz-transformation.md). Thus the formula gives the [Lorentz spinor double cover](../../../../../lorentz-spinor-double-cover.md)

$$
\boxed{SL(2,\mathbb C)/\{\pm I\}\cong SO^+(1,3).}
$$

It is a map into $SO(1,3)$ as asked, with precisely its identity component as image; it does not produce disconnected time-reversing transformations.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
