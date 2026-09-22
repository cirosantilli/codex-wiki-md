<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The local matrix $U(x)$ is a [gauge transformation](../../../../../gauge-transformation.md) in the [representation](../../../../../group-representation.md) acting on the matter field. With Hermitian [Lie algebra generators](../../../../../lie-algebra-generator.md) it can be written locally in spacetime, and pointwise for $SU(3)$, as

$$
U(x)=\exp[i\omega^a(x)T^a],\qquad [T^a,T^b]=if_{abc}T^c.
$$

The real functions $\omega^a$ can instead include a factor of $g$ by redefining the transformation parameters. The [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) convention in this paper is $D_\mu=\partial_\mu+igA_\mu$. Inserting the stated transformed $A_\mu$ shows explicitly that the $\partial_\mu U$ term cancels, giving $D_\mu'(U\psi)=UD_\mu\psi$.

In [QCD](../../../../../quantum-chromodynamics.md), each [quark field](../../../../../quark-field.md) is in the colour [fundamental representation](../../../../../fundamental-representation.md) $\mathbf3$, with $\psi^i\mapsto U^i{}_j\psi^j$. Thus its colour generators are **eight $3\times3$ matrices**, conventionally $T^a=\lambda^a/2$ for the [Gell-Mann matrices](../../../../../gell-mann-matrices.md); their number is not their matrix dimension. The eight [gluons](../../../../../gluon.md) themselves transform in the [adjoint representation of SU(3)](../../../../../adjoint-representation-of-su-3.md).

With $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$, the pure [Yang-Mills theory](../../../../../yang-mills-theory.md) has Lagrangian $\mathcal L_{\mathrm{YM}}=-\tfrac14F^a_{\mu\nu}F^{a\mu\nu}=-\tfrac12\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})$. Put $G^a_{\mu\nu}=\partial_\mu A^a_\nu-\partial_\nu A^a_\mu$ and $C^a_{\mu\nu}=f_{abc}A^b_\mu A^c_\nu$. Since $F=G-gC$,

$$
\mathcal L_{\mathrm{YM}}=-\frac14G^a_{\mu\nu}G^{a\mu\nu}+\frac g2G^a_{\mu\nu}C^{a\mu\nu}-\frac{g^2}4C^a_{\mu\nu}C^{a\mu\nu}.
$$

The cross term has two derivative contributions. Interchange $\mu,\nu$ and then $b,c$ in the second; antisymmetry of $f_{abc}$ makes it equal to the first. The [cubic and quartic Yang-Mills self-interactions](../../../../../cubic-and-quartic-yang-mills-self-interactions.md) are therefore

$$
\boxed{\mathcal L_3=gf_{abc}(\partial_\mu A^a_\nu)A^{b\mu}A^{c\nu},\qquad
\mathcal L_4=-\frac{g^2}4f_{abc}f_{ade}A^b_\mu A^c_\nu A^{d\mu}A^{e\nu}.}
$$

The positive cubic sign follows from the negative $gfAA$ term in the given [Yang-Mills field strength](../../../../../gauge-field-strength.md); changing the covariant-derivative convention consistently changes intermediate signs.

For the left-handed [quark doublet](../../../../../quark-doublet.md) $Q_L=(u_L,d_L)^T$, the [hypercharge](../../../../../hypercharge.md) is $Y=1/6$ and the weak generators are $\sigma^\alpha/2$. Its electroweak term is

$$
\boxed{\mathcal L_{Q_L}=\overline Q_L i\gamma^\mu\left[\partial_\mu+\frac{ig}{2}\sigma^\alpha\mathcal A_\mu^\alpha+\frac{ig'}6 B_\mu\right]Q_L.}
$$

The [Pauli matrices](../../../../../pauli-matrices.md) give diagonal entries $\pm\mathcal A^3$ and off-diagonal entries $\mathcal A^1\mp i\mathcal A^2$. Expanding the term gives

$$
\begin{aligned}
\mathcal L_{Q_L}={}&\bar u_Li\gamma^\mu\partial_\mu u_L+\bar d_Li\gamma^\mu\partial_\mu d_L\\
&-\frac{g'}6B_\mu(\bar u_L\gamma^\mu u_L+\bar d_L\gamma^\mu d_L)
-\frac g2\mathcal A^3_\mu(\bar u_L\gamma^\mu u_L-\bar d_L\gamma^\mu d_L)\\
&-\frac g2\left[(\mathcal A^1_\mu-i\mathcal A^2_\mu)\bar u_L\gamma^\mu d_L
+(\mathcal A^1_\mu+i\mathcal A^2_\mu)\bar d_L\gamma^\mu u_L\right].
\end{aligned}
$$

In particular the off-diagonal [weak charged current](../../../../../charged-current.md) coupling is $-g(W_\mu\bar u_L\gamma^\mu d_L+W_\mu^*\bar d_L\gamma^\mu u_L)/\sqrt2$.

Write $s_W=\sin\theta_W$, $c_W=\cos\theta_W$. Invert the neutral-field rotation: $\mathcal A^3_\mu=c_WZ_\mu+s_WA_\mu$, $B_\mu=c_WA_\mu-s_WZ_\mu$. The original PDF gives $\tan\theta_W=g'/g$, so

$$
\boxed{e=g\sin\theta_W=g'\cos\theta_W.}
$$

The [photon](../../../../../photon.md) coefficients inside the derivative are $gs_W/2+g'c_W/6=2e/3$ for $u_L$, and $-gs_W/2+g'c_W/6=-e/3$ for $d_L$. Multiplication by the $i$ in the kinetic Lagrangian gives the requested [electromagnetic coupling of a weak multiplet](../../../../../electromagnetic-coupling-of-a-weak-multiplet.md):

$$
\boxed{\mathcal L_{\mathrm{em}}=-\frac23e\bar u_LA_\mu\gamma^\mu u_L+\frac13e\bar d_LA_\mu\gamma^\mu d_L.}
$$

Equivalently it is $-eA_\mu\overline Q_L\gamma^\mu(T_3+Y)Q_L$, making the [electric charges](../../../../../electric-charge.md) explicit. The remaining neutral terms are $-(g/c_W)Z_\mu\{(1/2-2s_W^2/3)\bar u_L\gamma^\mu u_L+(-1/2+s_W^2/3)\bar d_L\gamma^\mu d_L\}$. The TeX's missing prime in the mixing-angle ratio and truncated first Pauli matrix are conversion errors, not physical assumptions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
