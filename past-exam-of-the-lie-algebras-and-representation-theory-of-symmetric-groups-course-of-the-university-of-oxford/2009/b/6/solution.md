<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the standard invariant [tabloid bilinear form](../../../../tabloid-bilinear-form.md), with the [tabloid](../../../../tabloid.md) [basis](../../../../basis.md) orthonormal. Each permutation acts by an orthogonal [matrix](../../../../matrix.md), so $\langle gx,y\rangle=\langle x,g^{-1}y\rangle$. Inversion permutes $C_t$ and preserves its signs. Therefore

$$
\boxed{\langle\kappa_tx,y\rangle=\sum_{g\in C_t}\operatorname{sgn}(g)\langle x,g^{-1}y\rangle=\langle x,\kappa_ty\rangle.}
$$

The [James submodule theorem](../../../../james-submodule-theorem.md) states that for any submodule $U\leq M^\lambda$, either $S^\lambda\subseteq U$ or $U\subseteq(S^\lambda)^\perp$. Use the allowed fact $\kappa_tM^\lambda=Fe_t$. The coefficient of $\{t\}$ in $e_t$ is one, so the displayed adjoint identity gives $\kappa_tx=\langle x,e_t\rangle e_t$. If $U$ is not orthogonal to $S^\lambda$, some $x\in U$ and some tableau $t$ have $\langle x,e_t\rangle\ne0$. Hence $e_t\in U$, and its permutation translates span $S^\lambda$. This proves the theorem.

Let $R=S^\lambda\cap(S^\lambda)^\perp$. Every proper submodule of $S^\lambda$ lies in $R$ by the theorem. If the restricted form is nonzero, $R$ is proper, hence is the unique maximal submodule and

$$
\boxed{D^\lambda=S^\lambda/R\text{ is the unique simple quotient}.}
$$

In the stronger nondegenerate case specified in the question, $R=0$, so $S^\lambda$ itself is simple. The nonzero-form version also covers the possibly degenerate case needed in the final calculation.

For shape $(n-1,1)$, identify $M$ with $F^n$ with [basis](../../../../basis.md) $v_1,\ldots,v_n$. Its [Specht module](../../../../specht-module.md) is the augmentation subspace $S=\{\sum a_iv_i:\sum a_i=0\}$, spanned freely by $v_i-v_n$, $1\leq i<n$. Its [Gram matrix](../../../../gram-matrix.md) is $G=I_{n-1}+J_{n-1}$, with diagonal entries two and off-diagonal entries one. Equivalently, $S^\perp$ in $M$ is the span of $v_1+\cdots+v_n$. This vector belongs to $S$ exactly when $p\mid n$. Thus the restricted radical has [dimension](../../../../dimension-vector-space.md) one if $p\mid n$ and zero otherwise, giving

$$
\boxed{\dim D^{(n-1,1)}=\begin{cases}n-2,&p\mid n,\\n-1,&p\nmid n.\end{cases}}
$$

For $n\geq3$ this quotient is nonzero and simple by the theorem. In the small exceptional case $n=2,p=2$, the canonical radical quotient is zero, as the same [dimension](../../../../dimension-vector-space.md) formula states; it is then not a nonzero [simple module](../../../../irreducible-module.md). This qualification distinguishes the numerical formula from the nonzero-form hypothesis.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
