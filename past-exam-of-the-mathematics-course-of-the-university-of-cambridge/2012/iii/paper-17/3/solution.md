<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Lie algebra](../../../../../lie-algebra-split.md) of a [Lie group](../../../../../lie-group.md) $G$ is the vector space $\mathfrak g=T_eG$ equipped with the bracket transferred from [left-invariant vector fields](../../../../../left-invariant-vector-field.md). For $a\in G$, write $L_a(g)=ag$. A field is left-invariant when $(D_gL_a)X_g=X_{ag}$ for all $a,g$. Given $v\in T_eG$, define

$$
X_v(g)=(D_eL_g)v.
$$

This is smooth and left-invariant, because $L_aL_g=L_{ag}$ and the [chain rule](../../../../../chain-rule.md) applies. Conversely a left-invariant field is determined by its value at $e$, through this formula. Thus

$$
\boxed{v\longmapsto X_v}
$$

is a vector-space isomorphism, whose inverse is evaluation at the identity.

The [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) is preserved by [diffeomorphisms](../../../../../diffeomorphism.md): on functions this follows by transporting the commutator of derivations. Therefore the bracket of two left-invariant fields is again left-invariant. Define $[v,w]=[X_v,X_w]_e$. Bilinearity, antisymmetry and the [Jacobi identity](../../../../../jacobi-identity.md) follow from the same properties of commutators of derivations. This supplies the asserted [Lie algebra](../../../../../lie-algebra-split.md) structure.

For the [general linear group](../../../../../general-linear-group.md) $GL_n(\mathbb R)$, invertible matrices form an open subset of $M_n(\mathbb R)$, so $T_IGL_n(\mathbb R)=M_n(\mathbb R)$. The left-invariant field determined by $A$ is $X_A(g)=gA$. Its ambient derivative is $D_gX_A(H)=HA$. Therefore [differentiating left-invariant matrix fields](../../../../../differentiating-left-invariant-matrix-fields.md) gives

$$
[X_A,X_B](g)=D_gX_B(gA)-D_gX_A(gB)=g(AB-BA).
$$

Hence

$$
\boxed{\mathfrak{gl}_n(\mathbb R)=M_n(\mathbb R),\qquad[A,B]=AB-BA.}
$$

This is the [general linear Lie algebra](../../../../../general-linear-lie-algebra.md), with the ordinary [matrix commutator](../../../../../commutator.md); right invariance with the same identification would give the opposite sign.

Now let $F:G\to H$ be a smooth [Lie group homomorphism](../../../../../lie-group-homomorphism.md). It sends the identity to the identity and induces the linear map

$$
F_*=D_eF:T_eG\to T_eH.
$$

Since $F\circ L_g=L_{F(g)}\circ F$, differentiation gives

$$
(D_gF)X_v(g)=X_{F_*v}(F(g)).
$$

These fields are $F$-related; no injectivity or surjectivity of $F$ is needed. For every smooth function $f$ on $H$,

$$
X_v(f\circ F)=(X_{F_*v}f)\circ F.
$$

Apply this first with $w$ and then with $v$, and subtract the reversed order. The result is

$$
[X_v,X_w](f\circ F)=([X_{F_*v},X_{F_*w}]f)\circ F.
$$

At $e$, smooth functions detect tangent vectors, so

$$
\boxed{F_*[v,w]=[F_*v,F_*w].}
$$

This proves that the [differential of a Lie group homomorphism preserves Lie brackets](../../../../../differential-of-a-lie-group-homomorphism-preserves-lie-brackets.md), and hence that $F_*$ is a [Lie algebra homomorphism](../../../../../lie-algebra-homomorphism.md).

For the exponential identity, let $\eta_v$ be the integral curve of $X_v$ through $e$. Left invariance and uniqueness show $\eta_v(t+s)=\eta_v(t)\eta_v(s)$ for small times: translating the curve through $e$ gives the curve through $\eta_v(s)$. Repeating this identity extends the curve to all real times. This proves [completeness of left-invariant vector fields](../../../../../completeness-of-left-invariant-vector-fields.md) without assuming that an arbitrary smooth field is complete. Rescaling the parameter also gives $\eta_v(t)=\eta_{tv}(1)$. By the definition of the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md), $\exp_G(v)=\eta_v(1)$.

The field-related identity shows that $F(\eta_v(t))$ is an integral curve of $X_{F_*v}$ starting at $e_H$. By uniqueness it equals $\eta_{F_*v}(t)$ for all times. At time one,

$$
\boxed{F(\exp_Gv)=\exp_H(F_*v).}
$$

This is the [naturality of the Lie group exponential](../../../../../naturality-of-the-lie-group-exponential.md).

Apply this to the [determinant](../../../../../determinant.md) homomorphism $GL_n(\mathbb R)\to\mathbb R^\times$. The derivative of the determinant at $I$ is

$$
D_I\det(A)=\operatorname{tr}A,
$$

since the permutation formula gives $\det(I+tA)=1+t\operatorname{tr}A+O(t^2)$. The left-invariant field on $\mathbb R^\times$ with initial tangent $c$ is $y\mapsto cy$; its curve through one solves $y'=cy$, hence is $e^{ct}$. The [matrix exponential determinant identity](../../../../../matrix-exponential-determinant-identity.md) therefore follows from naturality:

$$
\boxed{\det(\exp A)=e^{\operatorname{tr}A}.}
$$

This argument uses only the flow definition of the exponential and the scalar exponential, not an unproved matrix formula.

To identify it explicitly with the usual [matrix exponential](../../../../../matrix-exponential.md), the series $E(t)=\sum_{k\geq0}t^kA^k/k!$ converges in [operator norm](../../../../../operator-norm.md), uniformly with its differentiated series on bounded intervals. Termwise differentiation gives $E'=EA$ and $E(0)=I$. The series commutes with $A$, and differentiating $E(t)E(-t)$ gives zero, so $E(t)E(-t)=I$. Thus $E(t)$ stays in $GL_n(\mathbb R)$ and, by uniqueness, is the integral curve of $X_A$ through $I$. **The matrix series is exactly the flow-defined exponential**, justifying either notation in the determinant identity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
