<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

If a [vector bundle](../../../../../vector-bundle.md) $E\to M$ has rank $k$, form the [exterior power of a vector bundle](../../../../../exterior-power-of-a-vector-bundle.md) fibrewise: its fibre at $p$ is $\Lambda^rE_p$. A [vector bundle trivialization](../../../../../vector-bundle-trivialization.md) over $U$ induces one with fibre $\Lambda^r\mathbb R^k$. Transition matrices $A_{\alpha\beta}(p)$ induce $\Lambda^rA_{\alpha\beta}(p)$, which are smooth and obey the cocycle law because exterior powers preserve composition. They glue to a smooth bundle of rank $\binom{k}{r}$; for $r>k$ it is the zero bundle. At $r=k$ it is the [determinant line bundle](../../../../../determinant-line-bundle.md).

A real [line bundle](../../../../../line-bundle.md) is trivial precisely when it has a nowhere-zero smooth section: a section $s$ gives the bundle isomorphism $(p,t)\mapsto ts(p)$ from $M\times\mathbb R$. Apply this to $\Lambda^nT^*M$. Suppose first that an [oriented atlas](../../../../../oriented-atlas.md) is given. Its local coordinate forms

$$
\nu_\alpha=dx_\alpha^1\wedge\cdots\wedge dx_\alpha^n
$$

are positive multiples of one another on every overlap. Choose a subordinate smooth [partition of unity](../../../../../partition-of-unity.md) $\rho_\alpha\ge0$. Extend $\rho_\alpha\nu_\alpha$ by zero outside its chart and set $\nu=\sum_\alpha\rho_\alpha\nu_\alpha$. Local finiteness makes this smooth. At any point at least one weight is positive, and all summands are nonnegative multiples of the same positive top form. Therefore $\nu$ never vanishes, proving triviality of the line bundle.

Conversely let $\nu$ be a nowhere-zero section of $\Lambda^nT^*M$. In each sufficiently small connected chart write $\nu=a_\alpha\,dx_\alpha^1\wedge\cdots\wedge dx_\alpha^n$. Its coefficient has constant nonzero sign. If necessary reverse the first coordinate, making $a_\alpha>0$. On overlaps the equality of the two expressions gives

$$
a_\alpha\det\left(\frac{\partial x_\alpha}{\partial x_\beta}\right)=a_\beta,
$$

so each transition determinant is positive. These charts cover $M$, proving

$$
\boxed{\Lambda^nT^*M\text{ trivial}\quad\Longleftrightarrow\quad M\text{ admits an oriented atlas}.}
$$

For dimension zero both assertions hold with the empty exterior product equal to one.

For the [orientability of a vector bundle total space](../../../../../orientability-of-a-vector-bundle-total-space.md), write $\pi:E\to M$, with rank $r$ and orientable base. The vertical tangent vectors at $v\in E_p$ identify with $E_p$ by differentiating translation in that fibre. The differential of $\pi$ therefore gives the exact sequence of vector bundles on $E$

$$
0\longrightarrow\pi^*E\longrightarrow TE\xrightarrow{d\pi}\pi^*TM\longrightarrow0.
$$

Taking [determinant line bundles](../../../../../determinant-line-bundle.md) gives

$$
\det TE\cong\pi^*(\det E\otimes\det TM).
$$

To see the determinant identification directly, wedge a vertical frame with any lifts of a base frame; altering a lift by a vertical vector does not change that top wedge. Since $M$ is orientable, $\det TM$ is trivial. Consequently $\det TE\cong\pi^*\det E$. If $\det E$ is trivial, so is its pullback, making the total space orientable. Conversely, if $E$ is orientable as a manifold, its tangent determinant is trivial; restricting this isomorphism to the [zero section](../../../../../zero-section-of-a-vector-bundle.md) gives triviality of $\det E$. The tangent and cotangent determinant lines are dual, so either tests orientability. We obtain

$$
\boxed{E\text{ orientable as a manifold}\quad\Longleftrightarrow\quad\Lambda^rE\text{ trivial},\quad\text{when }M\text{ is orientable}.}
$$

For a [cotangent bundle](../../../../../cotangent-bundle.md) the base need not be orientable. If base coordinates change from $x$ to $y=y(x)$ with Jacobian $J$, fibre coordinates of the same covector change from $\xi$ to $\eta=J^{-T}\xi$. The full coordinate change on $T^*M$ has block Jacobian

$$
\begin{pmatrix}J&0\\ *&J^{-T}\end{pmatrix},\qquad\det J\det J^{-T}=1>0.
$$

Thus every induced cotangent coordinate change preserves orientation, even when the base change reverses it. These charts form an [oriented atlas](../../../../../oriented-atlas.md) on the total space, proving **every cotangent bundle is orientable**. Equivalently the canonical [symplectic form](../../../../../symplectic-form.md) of the [cotangent bundle](../../../../../cotangent-bundle.md) has a nowhere-zero top exterior power, as in [cotangent bundle orientation](../../../../../cotangent-bundle-orientation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
