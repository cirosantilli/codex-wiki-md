<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A smooth [vector field](../../../../../vector-field.md) on a [smooth manifold](../../../../../smooth-manifold.md) $M$ is a smooth section $X:M\to TM$ of its [tangent bundle](../../../../../tangent-bundle.md). It acts on smooth functions by $Xh(p)=dh_p(X_p)$. In a [manifold chart](../../../../../manifold-chart.md), $X=\sum_iX^i\partial_i$. The [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) is the commutator of their actions on functions:

$$
[X,Y]h=X(Yh)-Y(Xh).
$$

Expanding in coordinates makes all second derivatives cancel and gives

$$
[X,Y]=\sum_i\left(\sum_jX^j\partial_jY^i-Y^j\partial_jX^i\right)\partial_i.
$$

Thus the commutator is again a smooth [vector field](../../../../../vector-field.md), not a second-order operator. The coordinate expression represents the intrinsic derivation on functions, so agrees on overlaps.

For a [diffeomorphism](../../../../../diffeomorphism.md) $f:M\to N$, its [pushforward of a vector field](../../../../../pushforward-of-a-vector-field.md) is

$$
(f_*X)_q=df_{f^{-1}(q)}X_{f^{-1}(q)}.
$$

For every smooth function $h$ on $N$, the [chain rule](../../../../../chain-rule.md) gives $((f_*X)h)\circ f=X(h\circ f)$. Applying this twice yields

$$
([f_*X,f_*Y]h)\circ f=X(Y(h\circ f))-Y(X(h\circ f))=([X,Y](h\circ f))=((f_*[X,Y])h)\circ f.
$$

Smooth functions determine a tangent vector, and $f$ is surjective, so

$$
\boxed{f_*[X,Y]=[f_*X,f_*Y].}
$$

On a [Lie group](../../../../../lie-group.md), a [left-invariant vector field](../../../../../left-invariant-vector-field.md) satisfies $(L_g)_*X=X$ for every left translation $L_g(h)=gh$. Given $\xi\in T_eG$, set

$$
X_\xi(g)=(dL_g)_e\xi.
$$

This field is smooth by smoothness of multiplication. The equality $L_aL_g=L_{ag}$ proves left invariance. Conversely, left invariance forces $X(g)=(dL_g)_eX(e)$, so $X_\xi$ is the unique left-invariant field with value $\xi$ at $e$. This is a linear isomorphism between $T_eG$ and the space of [left-invariant vector fields](../../../../../left-invariant-vector-field.md).

The pushforward identity applied to $L_g$ shows that $[X_\xi,X_\eta]$ is again left invariant. Consequently

$$
[\xi,\eta]=[X_\xi,X_\eta](e)
$$

defines a [Lie bracket](../../../../../lie-bracket.md) on $T_eG$. Bilinearity and antisymmetry follow from the operator commutator. Its [Jacobi identity](../../../../../jacobi-identity.md) follows by expanding the three nested commutators: the six triple compositions cancel in pairs. These properties transfer through the linear isomorphism, making $T_eG$ the [Lie algebra](../../../../../lie-algebra-split.md) of $G$.

For the [general linear group](../../../../../general-linear-group.md) $G=\mathrm{GL}(n,\mathbb R)$, use matrix-entry coordinates $x_{pq}$. It is an open subset of $M_n(\mathbb R)$, so every tangent space is naturally $M_n(\mathbb R)$. Since $L_g(h)=gh$, its differential sends $A$ to $gA$, and hence

$$
X_A=\sum_{p,q}(gA)_{pq}\frac{\partial}{\partial x_{pq}},\qquad X_A(x_{pq})=\sum_kx_{pk}A_{kq}.
$$

For $A,B\in M_n(\mathbb R)$,

$$
X_A(X_B(x_{pq}))=\sum_k(gA)_{pk}B_{kq}=(gAB)_{pq},
$$

and reversing $A,B$ gives $(gBA)_{pq}$. Thus $[X_A,X_B]=X_{AB-BA}$; evaluating at the identity gives the [matrix commutator](../../../../../commutator.md)

$$
\boxed{[A,B]=AB-BA.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
