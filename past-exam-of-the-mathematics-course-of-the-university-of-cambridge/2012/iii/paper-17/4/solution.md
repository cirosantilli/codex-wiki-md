<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) $E\to M$ is an $\mathbb R$-linear map

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E)
$$

satisfying $\nabla(fs)=df\otimes s+f\nabla s$. Equivalently its directional version is real-bilinear and satisfies

$$
\nabla_{fX}s=f\nabla_Xs,\qquad
\nabla_X(fs)=X(f)s+f\nabla_Xs.
$$

For a complex bundle it is complex-linear in the section variable and has the same Leibniz property.

Every smooth vector bundle over an ordinary Hausdorff, second-countable [smooth manifold](../../../../../smooth-manifold.md) has such a connection. Choose trivializing open sets $U_a$, local frames $e_{a,i}$ and a subordinate locally finite [partition of unity](../../../../../partition-of-unity.md) $\rho_a$. In each frame define the flat local connection

$$
\nabla^{(a)}\left(\sum_i f_i e_{a,i}\right)=\sum_i df_i\otimes e_{a,i}.
$$

Then set $\nabla s=\sum_a\rho_a\nabla^{(a)}(s|_{U_a})$, extending each weighted term by zero outside $U_a$. The supports lie inside the corresponding trivializing sets, making the extensions smooth, and local finiteness makes the sum smooth. Since $\sum_a\rho_a=1$, its Leibniz rule is

$$
\nabla(fs)=\sum_a\rho_a(df\otimes s+f\nabla^{(a)}s)
=df\otimes s+f\nabla s.
$$

This is the [construction of a vector bundle connection by a partition of unity](../../../../../construction-of-a-vector-bundle-connection-by-a-partition-of-unity.md).

The difference $A=\nabla'-\nabla$ of two connections is $C^\infty(M)$-linear in both its vector-field argument and its section argument. The derivative terms cancel, so $A_Xs$ depends only on $X_p,s_p$ at each point. Smooth local coefficients therefore identify it with

$$
A\in\Omega^1(M;\operatorname{End}E)
=\Gamma(T^*M\otimes\operatorname{End}E).
$$

Conversely, any such $A$ added to a connection preserves its axioms. Thus **connections form an affine space modeled on $\Omega^1(M;\operatorname{End}E)$**. Choosing a base connection $\nabla^0$ gives the noncanonical bijection $A\mapsto\nabla^0+A$; there is no distinguished zero connection and hence no canonical vector-space identification. This is the [affine space of vector-bundle connections](../../../../../affine-space-of-vector-bundle-connections.md).

For a connection on $TM$, the [torsion tensor](../../../../../torsion-tensor.md) is the alternating operation $\tau(X,Y)=\nabla_XY-\nabla_YX-[X,Y]$. The connection and bracket Leibniz rules give

$$
\begin{aligned}
\tau(fX,Y)
&=f\nabla_XY-\bigl(Y(f)X+f\nabla_YX\bigr)
-\bigl(f[X,Y]-Y(f)X\bigr)\\
&=f\tau(X,Y).
\end{aligned}
$$

Alternation then gives $\tau(X,fY)=f\tau(X,Y)$ as well. Hence it is tensorial, of type one contravariant and two covariant indices:

$$
\boxed{\tau\in\Gamma(TM\otimes\Lambda^2T^*M).}
$$

It is equivalently a $TM$-valued two-form, a [torsion form](../../../../../torsion-form.md).

For the local frame $e_i$ with dual [coframe](../../../../../coframe.md) $\phi_j$, define

$$
\omega_{ij}(X)=\phi_j(\nabla_Xe_i).
$$

The connection is $C^\infty$-linear in $X$, so these are smooth [differential one-forms](../../../../../one-form.md). Expansion in the frame gives $\nabla_Xe_i=\sum_j\omega_{ij}(X)e_j$, and uniqueness follows by applying each $\phi_j$. Here the first index is the input frame vector and the second the output coefficient; this fixes the [connection one-form](../../../../../connection-one-form.md) convention.

Expand $Y=\sum_i\phi_i(Y)e_i$ and apply the connection Leibniz rule:

$$
\phi_j(\nabla_XY)=X(\phi_j(Y))+\sum_i\phi_i(Y)\omega_{ij}(X).
$$

Subtract the corresponding expression with $X,Y$ exchanged, and then subtract $\phi_j([X,Y])$. By the [exterior derivative of a one-form evaluated on vector fields](../../../../../exterior-derivative-of-a-one-form-evaluated-on-vector-fields.md),

$$
\begin{aligned}
\tau_j(X,Y)
&=d\phi_j(X,Y)
+\sum_i\bigl(\phi_i(Y)\omega_{ij}(X)-\phi_i(X)\omega_{ij}(Y)\bigr)\\
&=\left(d\phi_j-\sum_i\phi_i\wedge\omega_{ij}\right)(X,Y).
\end{aligned}
$$

Since all pairs of tangent vectors can be tested, equality of the two-forms follows:

$$
\boxed{d\phi_j=\sum_i\phi_i\wedge\omega_{ij}+\tau_j.}
$$

This is the [Cartan first structure equation with input-first indices](../../../../../cartan-first-structure-equation-with-input-first-indices.md). Its plus sign is correct with the stated index order and wedge order; the common output-first convention writes the same identity with a minus sign and reversed wedge factors.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
