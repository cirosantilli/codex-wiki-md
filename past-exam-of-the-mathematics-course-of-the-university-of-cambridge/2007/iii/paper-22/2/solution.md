<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On a [complex manifold](../../../../../complex-manifold.md), [holomorphic coordinates](../../../../../holomorphic-coordinate.md) give the decomposition $d=\partial+\bar\partial$, with

$$
\partial:\mathcal A^{p,q}\to\mathcal A^{p+1,q},\qquad
\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1}.
$$

For $\alpha=\sum_{I,J}a_{I\bar J}\,dz^I\wedge d\bar z^J$, the [conjugate Dolbeault operator](../../../../../conjugate-dolbeault-operator.md) $\partial$ and the [Dolbeault operator](../../../../../dolbeault-operator.md) $\bar\partial$ are explicitly

$$
\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I\bar J}}{\partial z^k}\,dz^k\wedge dz^I\wedge d\bar z^J,
\qquad
\bar\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I\bar J}}{\partial\bar z^k}\,d\bar z^k\wedge dz^I\wedge d\bar z^J.
$$

These are the type components of the intrinsic [exterior derivative](../../../../../exterior-derivative.md), so are independent of coordinates. The identity $d^2=0$, separated by type, gives $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$. A [holomorphic p-form on a complex manifold](../../../../../holomorphic-p-form-on-a-complex-manifold.md) is a $(p,0)$-form whose coefficients are [holomorphic functions](../../../../../holomorphic-function.md); equivalently it is a $(p,0)$-form killed by the [Dolbeault operator](../../../../../dolbeault-operator.md).

A rank-$r$ [holomorphic vector bundle](../../../../../holomorphic-vector-bundle.md) has local trivializations $E|_{U_i}\cong U_i\times\mathbb C^r$ whose changes are $(x,v)\mapsto(x,g_{ij}(x)v)$, with $g_{ij}:U_i\cap U_j\to\operatorname{GL}_r(\mathbb C)$ holomorphic. These [transition functions of a vector bundle](../../../../../transition-function-of-a-vector-bundle.md) satisfy $g_{ii}=I$ and $g_{ij}g_{jk}=g_{ik}$. Equivalently, for local frames we use the convention $e_j=e_i g_{ij}$. A [holomorphic section](../../../../../holomorphic-section.md) is a section having holomorphic coordinate functions in every such [holomorphic local frame](../../../../../holomorphic-local-trivialization.md); the condition is unchanged by the holomorphic invertible transitions.

The [holomorphic cotangent bundle](../../../../../holomorphic-cotangent-bundle.md) has local frames $dz^1,\ldots,dz^n$. Under another [holomorphic coordinate](../../../../../holomorphic-coordinate.md) system $w$, the [chain rule](../../../../../chain-rule.md) gives

$$
dw^a=\sum_b\frac{\partial w^a}{\partial z^b}\,dz^b.
$$

The Jacobian matrix is holomorphic and invertible, with holomorphic inverse supplied by the inverse coordinate change. These are precisely holomorphic bundle transitions. A section written as $\sum_b f_b(z)\,dz^b$ is holomorphic exactly when every $f_b$ is holomorphic, so

$$
\boxed{H^0(X,\Omega_X^1)=\{\alpha\in\mathcal A^{1,0}(X):\bar\partial\alpha=0\},}
$$

the space of [holomorphic one-forms](../../../../../holomorphic-one-form.md). In particular, being a holomorphic section is not the same as being a $d$-closed one-form on an arbitrary [complex manifold](../../../../../complex-manifold.md).

The [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) is

$$
\mathcal O(-1)=\{([Z],v)\in\mathbb{CP}^n\times\mathbb C^{n+1}:v\in\mathbb C Z\}.
$$

On $U_i=\{Z_i\ne0\}$ use the nowhere-zero frame $s_i([Z])=Z/Z_i$. Its components are holomorphic affine coordinates and the constant one in position $i$. On overlaps

$$
s_j=\frac{Z_i}{Z_j}s_i,
$$

so the frame changes are nowhere-zero [holomorphic functions](../../../../../holomorphic-function.md). This proves that $\mathcal O(-1)$ is a [holomorphic line bundle](../../../../../holomorphic-line-bundle.md), and its inclusion into the trivial bundle is a [holomorphic bundle map](../../../../../holomorphic-bundle-map.md).

A global [holomorphic section](../../../../../holomorphic-section.md) composed with that inclusion has $n+1$ component [holomorphic functions](../../../../../holomorphic-function.md) on compact connected [Complex projective space](../../../../../complex-projective-space.md). Each is constant: its absolute value attains a maximum; in a coordinate ball the one-variable maximum modulus principle along complex lines makes it locally constant, and connectedness propagates that constant globally. Thus the section is a fixed vector $v\in\mathbb C^{n+1}$ lying in every fibre, namely every line $\mathbb C Z$. For $n\geq1$ the intersection of all these lines is zero. Hence

$$
\boxed{H^0(\mathbb{CP}^n,\mathcal O(-1))=0\quad(n\geq1).}
$$

The positive-dimension convention is necessary: $\mathbb{CP}^0$ is one point and this section space is $\mathbb C$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
