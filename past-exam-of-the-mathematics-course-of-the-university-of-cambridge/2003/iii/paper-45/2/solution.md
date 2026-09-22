<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The invariant [tensors](../../../../../tensor.md) of [SU(3)](../../../../../su-3-group.md) include $\delta^\alpha_\beta$, $\epsilon_{\alpha\beta\gamma}$ and its upper-index counterpart. Consequently an antisymmetric pair of upper fundamental indices can be converted into one lower antifundamental index, and conversely; a completely antisymmetric triple is a determinant singlet. In the [Young-symmetrizer tensor decomposition](../../../../../young-symmetrizer-tensor-decomposition.md), complete columns of three can therefore be removed. A remaining diagram has rows of lengths $k+l,l$: its two-box columns become $l$ dual indices and its remaining boxes give $k$ defining indices. The irreducible highest-weight component is represented by a [mixed SU(3) tensor representation](../../../../../mixed-su-3-tensor-representation.md) symmetric in all upper indices, symmetric in all lower indices, and with every upper-lower contraction removed. Such contractions produce the lower-weight components. The resulting [symmetric traceless SU(3) tensor representation](../../../../../symmetric-traceless-su-3-tensor-representation.md) has [Dynkin labels](../../../../../dynkin-label.md) $(k,l)$; this is an equivalent canonical realization, not a claim that an arbitrary tensor already has those symmetries.

There are $\binom{k+2}{2}$ symmetric upper-index components and $\binom{l+2}{2}$ symmetric lower-index components. All contractions are equivalent under the separate symmetries. Their image is the separately symmetric tensor space with $(k-1,l-1)$ indices. To subtract its dimension legitimately, we must show that contraction is onto.

Represent such [tensors](../../../../../tensor.md) by polynomials of bidegree $(k,l)$ in three variables $x$ and three dual variables $y$. Up to a nonzero normalization, contraction is

$$
\Delta=\sum_{a=1}^3\partial_{x_a}\partial_{y_a},\qquad q=\sum_{a=1}^3x_ay_a.
$$

If $P$ has bidegree $(k-1,l-1)$, differentiation gives

$$
\Delta(q^{j+1}\Delta^jP)=q^{j+1}\Delta^{j+1}P+(j+1)(k+l+1-j)q^j\Delta^jP.
$$

Choose $a_0=1/(k+l+1)$ and $a_j=-a_{j-1}/[(j+1)(k+l+1-j)]$. Then

$$
Q=\sum_{j=0}^{\min(k-1,l-1)}a_jq^{j+1}\Delta^jP
$$

has bidegree $(k,l)$ and $\Delta Q=P$: consecutive terms cancel, and the last further derivative vanishes. This constructs a preimage of every contraction target. If $k=0$ or $l=0$, there is no contraction. Therefore the number of trace-free components is

$$
\begin{aligned}
\dim R(k,l)&=\binom{k+2}{2}\binom{l+2}{2}-\binom{k+1}{2}\binom{l+1}{2}\\
&=\frac14(k+1)(k+2)(l+1)(l+2)-\frac14k(k+1)l(l+1)\\
&=\boxed{\frac12(k+1)(l+1)(k+l+2)}.
\end{aligned}
$$

The [highest-weight vector](../../../../../highest-weight-vector.md) $x_1^ky_3^l$ lies in this kernel. The Young-symmetry construction identifies the traceless highest-weight component with the [irreducible representation](../../../../../irreducible-representation.md) of labels $(k,l)$; equivalently its [Weyl dimension formula](../../../../../weyl-dimension-formula.md) agrees with the independently calculated kernel dimension above.

For traceless matrices $T,S$, the [tensor square of the SU(3) adjoint representation](../../../../../tensor-square-of-the-su-3-adjoint-representation.md) decomposes as

$$
\boxed{\mathbf8\otimes\mathbf8=\mathbf1\oplus\mathbf8_S\oplus\mathbf8_A\oplus\mathbf{10}\oplus\overline{\mathbf{10}}\oplus\mathbf{27}.}
$$

The component maps make the decomposition concrete. The singlet is $\operatorname{tr}(TS)$. The two octets are the antisymmetric [commutator](../../../../../commutator.md) $[T,S]$ and symmetric traceless anticommutator $\{T,S\}-\tfrac23\operatorname{tr}(TS)I$. Symmetrizing the two upper and two lower indices in $T^\alpha_\beta S^\gamma_\delta$ and removing contractions gives $R(2,2)$, the 27. Its highest component is already visible in $E_{13}\otimes E_{13}$.

For the 10, contract the two lower indices with $\epsilon^{\beta\delta\rho}$ and symmetrize the three upper indices $\alpha,\gamma,\rho$; for its conjugate, contract the upper pair with $\epsilon_{\alpha\gamma\rho}$ and symmetrize the three lower indices. These maps are antisymmetric under exchange of $T,S$. They are nonzero: $T=E_{12},S=E_{13}$ produces a nonzero all-upper-1 component, and $T=E_{21},S=E_{31}$ produces the conjugate all-lower-1 component. Thus they reach the irreducible $R(3,0)$ and $R(0,3)$, each of dimension ten. The octet maps are also nonzero, for example on a pair of noncommuting matrix units and on equal nonzero traceless diagonal matrices. These equivariant maps supply distinct irreducible constituents, with the two octets separated by exchange symmetry. Their dimensions exhaust the product:

$$
\dim\operatorname{Sym}^2\mathbf8=36=1+8+27,\qquad\dim\bigwedge^2\mathbf8=28=8+10+10,\qquad36+28=64.
$$

An octet operator between [baryon octet](../../../../../baryon-octet.md) states defines an [intertwining operator](../../../../../intertwining-operator.md) $\mathbf8_{\mathrm{operator}}\otimes\mathbf8_{\mathrm{state}}\to\mathbf8_{\mathrm{state}}$. Its covariance follows from the commutator transformation law in the question. By [Schur lemma](../../../../../schur-s-lemma.md), the number of independent [reduced matrix elements](../../../../../reduced-matrix-element.md) is the multiplicity of the output octet in the product: **there are exactly two independent coefficients**. To display them, use a Hermitian octet matrix basis $B_s=\lambda_s$, $t_i=\lambda_i/2$, normalized by $\operatorname{tr}(\lambda_r\lambda_s)=2\delta_{rs}$. The two allowed actions are

$$
B\longmapsto F[t_i,B]+D\left(\{t_i,B\}-\frac23\operatorname{tr}(t_iB)I\right).
$$

With $[\lambda_i,\lambda_s]=2if_{isk}\lambda_k$ and $\{\lambda_i,\lambda_s\}=\tfrac43\delta_{is}I+2d_{isk}\lambda_k$, this gives the [two reduced octet matrix elements](../../../../../two-reduced-octet-matrix-elements.md):

$$
\boxed{\langle B_r|V_i|B_s\rangle=Dd_{ris}+iFf_{ris},}
$$

up to the common normalization absorbed into $F,D$. All component dependence is fixed by the invariant symmetric and antisymmetric tensors. For a Hermitian operator and this Hermitian basis, $F,D$ may be chosen real; neither their values nor a relation between them follows from symmetry alone.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
