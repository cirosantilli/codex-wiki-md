<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [vector field](../../../../../vector-field.md) is a smooth section $X:M\to TM$ of the [tangent bundle](../../../../../tangent-bundle.md). It differentiates smooth functions by $Xf(p)=X_p(f)$. Define the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) intrinsically by

$$
\boxed{[X,Y]f=X(Yf)-Y(Xf).}
$$

Expanding this expression on a product $fh$ shows that the two mixed terms cancel, giving $[X,Y](fh)=f[X,Y]h+h[X,Y]f$. It is therefore a derivation, hence a [vector field](../../../../../vector-field.md). In local coordinates,

$$
[X,Y]=\sum_i\left(\sum_jX^j\partial_jY^i-Y^j\partial_jX^i\right)\partial_i.
$$

Its coefficients are smooth. The intrinsic definition depends on no chart, which proves coordinate independence of this formula and defines the bracket on the whole manifold.

For a [Lie group](../../../../../lie-group.md) $G$, let $L_g(h)=gh$ be [Left translation on a Lie group](../../../../../left-and-right-translation-on-a-lie-group.md). A [left-invariant vector field](../../../../../left-invariant-vector-field.md) satisfies $(dL_g)_hX_h=X_{gh}$ for every $g,h$. Evaluation $X\mapsto X_e$ is linear and injective, since $X_g=(dL_g)_eX_e$. Conversely any $B\in T_eG$ gives a smooth [left-invariant vector field](../../../../../left-invariant-vector-field.md) $X_B(g)=(dL_g)_eB$. Smoothness follows from smooth multiplication and its differential. Thus

$$
\boxed{\{\text{left-invariant vector fields on }G\}\cong T_eG.}
$$

For any [diffeomorphism](../../../../../diffeomorphism.md) $F$, the intrinsic bracket identity on functions gives $F_*[X,Y]=[F_*X,F_*Y]$. Applying this [naturality of the Lie bracket](../../../../../differential-of-a-lie-group-homomorphism-preserves-lie-brackets.md) to $F=L_g$ proves that the bracket of two [left-invariant vector fields](../../../../../left-invariant-vector-field.md) remains left invariant. Evaluation at $e$ therefore defines the [Lie algebra](../../../../../lie-algebra-split.md) bracket on $\mathfrak g=T_eG$.

For the [special orthogonal group](../../../../../special-orthogonal-group.md), differentiation of $Q(t)^TQ(t)=I$ at $Q(0)=I$ gives $B^T+B=0$, so its [tangent space](../../../../../tangent-space.md) is contained in the [skew-symmetric matrices](../../../../../skew-symmetric-matrix.md). Conversely, for any such $B$, the [matrix exponential](../../../../../matrix-exponential.md) $Q(t)=e^{tB}$ satisfies $Q(t)^TQ(t)=I$ and lies in the determinant-one component, because $Q(0)=I$ and its determinant varies continuously in $\{\pm1\}$. Its initial derivative is $B$, proving

$$
\boxed{\mathfrak{so}(n)=\{B\in M_n(\mathbb R):B^T=-B\}.}
$$

For matrices, $X_B(Q)=QB$. Extend these fields to the open matrix group $\mathrm{GL}(n,\mathbb R)$, where the differential of $Q\mapsto QB$ in direction $H$ is $HB$. Hence

$$
[X_{B_1},X_{B_2}](Q)=DX_{B_2}(Q)[QB_1]-DX_{B_1}(Q)[QB_2]=Q(B_1B_2-B_2B_1).
$$

Restriction to the embedded [special orthogonal group](../../../../../special-orthogonal-group.md) preserves this bracket because the fields are tangent. Evaluating at $I$ gives **$[B_1,B_2]=B_1B_2-B_2B_1$**, the required bracket on the [Special orthogonal Lie algebra](../../../../../special-orthogonal-lie-algebra.md). The commutator is again skew symmetric. This calculation is [differentiating left-invariant matrix fields](../../../../../differentiating-left-invariant-matrix-fields.md); reversing the order of the two differentials would give the wrong sign.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
