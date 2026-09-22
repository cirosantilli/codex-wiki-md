<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At a [perfectly bonded elastic interface](../../../../../perfectly-bonded-elastic-interface.md) without an interfacial force, [displacement](../../../../../displacement.md) and [traction](../../../../../traction.md) are continuous:

$$
[u]=0,\qquad[\sigma]n=0.
$$

Tangential derivatives of the common [displacement](../../../../../displacement.md) trace are also continuous. Thus the jump of a piecewise constant [displacement gradient tensor](../../../../../displacement-gradient-tensor.md) annihilates every tangential vector, and has the form $\alpha\otimes n$. Taking its symmetric part shows that the [strain](../../../../../strain.md) jump is $B\alpha$, where

$$
(B\alpha)_{ij}=\tfrac12(\alpha_i n_j+\alpha_j n_i),
\qquad B^T\tau=\tau n.
$$

The adjoint formula follows from $\tau:B\alpha=(\tau n)\cdot\alpha$ for symmetric [stress tensors](../../../../../cauchy-stress-tensor.md). Tangential-tangential [strain](../../../../../strain.md) components are therefore common to all layers. Conversely, such gradient jumps can be realized by continuous piecewise affine [displacement](../../../../../displacement.md) in the layered geometry.

Take positive [elastic stiffness tensors](../../../../../elastic-stiffness-tensor.md) with their usual minor and major symmetries, and a positive comparison [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) $C^0$. A fictitious layer can have the same tangential displacement derivatives and the same [traction](../../../../../traction.md) as the physical layers. Hence $\varepsilon^r=\varepsilon^0+B\alpha^r$. The common [traction](../../../../../traction.md) condition gives

$$
B^TC^r(\varepsilon^0+B\alpha^r)=B^TC^0\varepsilon^0,
\qquad K^r\alpha^r=-B^T(C^r-C^0)\varepsilon^0,
$$

where $K^r=B^TC^rB$ is the positive [acoustic tensor](../../../../../acoustic-tensor.md), with components $K^r_{ik}=C^r_{ijkl}n_j n_l$. Solving for $\alpha^r$ gives

$$
\boxed{\varepsilon^r=\bigl[I-\widetilde\Gamma^r(C^r-C^0)\bigr]\varepsilon^0,
\qquad \widetilde\Gamma^r=B(K^r)^{-1}B^T.}
$$

Expanding the two occurrences of $B$ gives exactly the symmetrization over $(ij)$ and $(kl)$ in the [directional elastic strain Green operator](../../../../../directional-elastic-strain-green-operator.md) specified in the paper.

For any two layers, the inverse identity for their [acoustic tensors](../../../../../acoustic-tensor.md) proves the required resolvent relation without interchanging noncommuting [tensors](../../../../../tensor.md):

$$
\begin{aligned}
\widetilde\Gamma^r(C^r-C^s)\widetilde\Gamma^s
&=B(K^r)^{-1}(K^r-K^s)(K^s)^{-1}B^T\\
&=B\bigl[(K^s)^{-1}-(K^r)^{-1}\bigr]B^T\\
&=\boxed{\widetilde\Gamma^s-\widetilde\Gamma^r}.
\end{aligned}
$$

With $D_r=C^r-C^0$, this identity also gives $\widetilde\Gamma^0D_r\widetilde\Gamma^r=\widetilde\Gamma^0-\widetilde\Gamma^r$. Therefore

$$
\bigl[I+\widetilde\Gamma^0D_r\bigr]
\bigl[I-\widetilde\Gamma^rD_r\bigr]=I.
$$

These finite-dimensional operators are inverses. Define $A_r=[I+\widetilde\Gamma^0(C^r-C^0)]^{-1}$. Then $\varepsilon^r=A_r\varepsilon^0$, and averaging [strains](../../../../../strain.md) and [stresses](../../../../../stress.md) gives

$$
E=\langle A\rangle\varepsilon^0,
\qquad S=\langle CA\rangle\varepsilon^0.
$$

Eliminating the fictitious [strain](../../../../../strain.md) yields

$$
\boxed{C^{\mathrm{eff}}=\langle CA\rangle\langle A\rangle^{-1}.}
$$

All products have the displayed order; the [elastic stiffness tensors](../../../../../elastic-stiffness-tensor.md) need not commute.

It remains to justify the inverse and comparison independence. Consider two compatible equilibrated layer solutions with the same mean [strain](../../../../../strain.md). Their difference has zero common tangential-tangential [strain](../../../../../strain.md), so $\delta\varepsilon^r=B\beta^r$, with $\sum_r c_r\beta^r=0$ because $B$ is injective and the mean difference is zero. Their [traction](../../../../../traction.md) difference is one common vector $g$. Therefore

$$
\sum_r c_r\delta\varepsilon^r:C^r\delta\varepsilon^r
=\sum_r c_r\beta^r\cdot g=0.
$$

Positive [elastic energy](../../../../../elastic-energy.md) forces every $\delta\varepsilon^r$ to vanish. In particular, if $\langle A\rangle\varepsilon^0=0$, all physical layer [strains](../../../../../strain.md) vanish. Their common tangential components then force $\varepsilon^0=B\beta^0$, and their zero [traction](../../../../../traction.md) gives $K^0\beta^0=0$. Hence $\varepsilon^0=0$, proving that $\langle A\rangle$ is invertible. Finally, every positive choice of $C^0$ constructs the unique layer solution for the same $E$. Its averaged [stress](../../../../../stress.md) is unique, so **the displayed effective stiffness is independent of the fictitious comparison material**. This is the exact layered constitutive response, rather than a claim that piecewise constant fields meet arbitrary finite-body boundary data.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
