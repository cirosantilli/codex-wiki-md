<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First complexify the [Clifford algebra](../../../../../clifford-algebra.md) in $D=2n$ spacetime dimensions. Multiplying appropriate generators by $i$ converts the signature to the Euclidean form $\{\Gamma_a,\Gamma_b\}=2\delta_{ab}$ without changing the complex module dimension. Pair the generators into

$$
b_j=\frac12(\Gamma_{2j-1}+i\Gamma_{2j}),\qquad
b_j^\dagger=\frac12(\Gamma_{2j-1}-i\Gamma_{2j}),\qquad j=1,\ldots,n.
$$

The [Clifford algebra](../../../../../clifford-algebra.md) relations give

$$
\{b_i,b_j\}=\{b_i^\dagger,b_j^\dagger\}=0,\qquad\{b_i,b_j^\dagger\}=\delta_{ij}.
$$

The commuting occupation operators $N_j=b_j^\dagger b_j$ have eigenvalues zero or one. Choose a nonzero state killed by every $b_j$; repeated annihilation reaches such a state in any finite irreducible module. Acting with distinct creation operators produces the $2^n$ occupation states

$$
(b_1^\dagger)^{r_1}\cdots(b_n^\dagger)^{r_n}|0\rangle,\qquad r_j\in\{0,1\}.
$$

Their distinct occupation patterns make them linearly independent, and their span is invariant under every Clifford generator. Irreducibility therefore makes it the entire Dirac module. This derives the [even-dimensional Clifford spinor dimension](../../../../../even-dimensional-clifford-spinor-dimension.md):

$$
\boxed{\dim_{\mathbb C}S_{\rm Dirac}=2^n=2^{D/2}.}
$$

The [chirality matrix](../../../../../chirality-matrix.md) is a phase-adjusted product of all $2n$ generators. It squares to one, anticommutes with each generator and acts as occupation parity up to an overall sign. Its two eigenspaces each have $2^{n-1}$ states. The even Clifford algebra, and hence the connected spin group, preserves them, giving irreducible [Weyl spinors](../../../../../weyl-spinor.md) of complex dimension $2^{D/2-1}$. A [Majorana spinor](../../../../../majorana-spinor.md) imposes a reality condition only in signatures where it exists; simultaneous Majorana and Weyl conditions are not available in every even dimension.

In Lorentzian ten dimensions, the complex Dirac module has dimension $32$, and a Weyl module dimension $16$. A [Majorana-Weyl spinor](../../../../../majorana-weyl-spinor.md) is allowed and has $16$ real components before its equation of motion. The massless Dirac equation leaves eight physical gaugino polarizations. A ten-dimensional massless [gauge field](../../../../../gauge-field.md) also has $10-2=8$ physical polarizations. Thus [ten-dimensional super Yang-Mills theory](../../../../../ten-dimensional-super-yang-mills-theory.md) has eight bosonic and eight fermionic states per gauge generator, with sixteen real [supercharges](../../../../../supersymmetry-generator.md).

For [dimensional reduction](../../../../../dimensional-reduction.md), take a flat six-torus with periodic fermions and retain fields independent of its coordinates. Split $A_M$ into $A_\mu$ and six internal components $A_m$, $m=4,\ldots,9$. The latter are four-dimensional real adjoint [scalar fields](../../../../../scalar-field.md). Under the spin groups of the two factors, a ten-dimensional chiral spinor decomposes as

$$
\mathbf{16}_{\mathbb C}\longrightarrow(\mathbf2,\mathbf4)\oplus(\overline{\mathbf2},\overline{\mathbf4})
$$

for $\operatorname{Spin}(1,3)\times\operatorname{Spin}(6)$, with $\operatorname{Spin}(6)\simeq SU(4)$. The Majorana condition relates these conjugate pieces, leaving four independent four-dimensional [Weyl spinors](../../../../../weyl-spinor.md). The supersymmetry parameters reduce in exactly the same fashion: sixteen real charges are four four-dimensional supersymmetries. The resulting field content is

$$
\boxed{A_\mu,\quad4\text{ adjoint Weyl fermions},\quad6\text{ real adjoint scalars}:\quad\mathcal N=4\text{ Yang-Mills}.}
$$

The on-shell counts are $2+6=8$ bosonic and $4\times2=8$ fermionic states, as required. The internal spin group supplies the $SU(4)$ [R-symmetry](../../../../../r-symmetry.md) of the reduced action.

To derive its [scalar potential](../../../../../scalar-potential.md), use Hermitian gauge matrices and a positive trace inner product, with

$$
S_{10}=-\frac1{4g_{10}^2}\int d^{10}x\,\operatorname{tr}(F_{MN}F^{MN}),\qquad
F_{MN}=\partial_MA_N-\partial_NA_M-i[A_M,A_N].
$$

If the internal volume is $V_6$, integration gives $g_4^2=g_{10}^2/V_6$. Since internal derivatives vanish,

$$
F_{\mu m}=\partial_\mu A_m-i[A_\mu,A_m],\qquad F_{mn}=-i[A_m,A_n].
$$

With mostly-minus spacetime signature, $F_{\mu m}F^{\mu m}$ has an extra minus sign and the double sum over mixed indices gives a factor two. Rescale $A_\mu=g_4a_\mu$ and $A_m=g_4X_m$ to canonical fields. The resulting bosonic Lagrangian is

$$
\mathcal L_4=-\frac14\operatorname{tr}(f_{\mu\nu}f^{\mu\nu})
+\frac12\sum_m\operatorname{tr}(D_\mu X_mD^\mu X_m)
+\frac{g_4^2}{4}\sum_{m,n}\operatorname{tr}[X_m,X_n]^2,
$$

where $D_\mu X_m=\partial_\mu X_m-ig_4[a_\mu,X_m]$. A commutator of Hermitian matrices is anti-Hermitian, so the last term is minus a nonnegative [scalar potential](../../../../../scalar-potential.md):

$$
\boxed{V=\frac{g_4^2}{4}\sum_{m,n}\operatorname{tr}\bigl([X_m,X_n]^\dagger[X_m,X_n]\bigr)\geq0.}
$$

The sum is over ordered internal pairs; a sum over $m<n$ would instead have coefficient $g_4^2/2$. Trace normalization merely changes the matched gauge-coupling convention.

The origin attains zero potential, so the global minima are exactly

$$
\boxed{[X_m,X_n]=0\quad\text{for every }m,n.}
$$

For a compact connected gauge group, a commuting tuple is simultaneously conjugate into a [Cartan subalgebra](../../../../../cartan-subalgebra.md). Write $X_m=\sum_{a=1}^rx_m^aH_a$, where $r$ is the rank. Every choice of the $6r$ real numbers $x_m^a$ has zero potential. After the residual [Weyl group](../../../../../weyl-group.md) identifications, the classical [commuting-scalar vacua of four-dimensional N=4 Yang-Mills theory](../../../../../commuting-scalar-vacua-of-four-dimensional-n-4-yang-mills-theory.md) form $(\mathbb R^6)^r/\mathcal W$ in the four-dimensional theory. For $SU(N)$ one may describe them as six simultaneous diagonal matrices, with tracelessness and permutations of their common eigenvalue labels. Varying these eigenvalues changes gauge-invariant configurations while leaving $V=0$, proving the existence of genuine [flat directions of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md), not just gauge-equivalent directions. Generic values break the gauge group to its maximal torus; coincident eigenvalue vectors produce enhanced unbroken gauge symmetry. If one keeps a finite compact torus rather than the four-dimensional limit, large gauge transformations add periodic identifications of the Wilson-line coordinates.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
