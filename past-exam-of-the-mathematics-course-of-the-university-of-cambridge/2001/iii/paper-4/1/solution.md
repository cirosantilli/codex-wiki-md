<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mathcal U=(U_0,\ldots,U_m)$ be a finite [affine open cover](../../../../../affine-open-cover.md) of the [projective scheme](../../../../../projective-scheme.md) $X$. For a [coherent sheaf](../../../../../coherent-sheaf.md) $\mathcal F$, form the [Čech cochain complex](../../../../../cech-cochain-complex.md)

$$
\check C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}\Gamma(U_{i_0}\cap\cdots\cap U_{i_p},\mathcal F),\qquad
(\delta c)_{i_0\ldots i_{p+1}}=\sum_{j=0}^{p+1}(-1)^j c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

The two ways to omit any pair of indices have opposite signs, giving $\delta^2=0$. Its [cohomology groups](../../../../../cohomology-group.md) are

$$
\check H^p(\mathcal U,\mathcal F)=\ker\delta^p/\operatorname{im}\delta^{p-1}.
$$

A [projective scheme](../../../../../projective-scheme.md) over a [field](../../../../../field.md) is a [separated scheme](../../../../../separated-scheme.md). Finite intersections of its affine opens are affine, and a [coherent sheaf](../../../../../coherent-sheaf.md) is [quasi-coherent](../../../../../quasi-coherent-sheaf.md). Higher [sheaf cohomology](../../../../../sheaf-cohomology.md) of a quasi-coherent sheaf on an [affine scheme](../../../../../affine-scheme.md) vanishes. Thus this is an acyclic cover and the [acyclic cover theorem](../../../../../leray-s-theorem.md) identifies the displayed [Čech cohomology](../../../../../cech-cohomology.md) with $H^p(X,\mathcal F)$. In particular its degree-zero kernel glues compatible local sections to $\Gamma(X,\mathcal F)$. A cover by $m+1$ opens also gives vanishing for $p>m$.

For the [cohomology of twists on projective space](../../../../../cohomology-of-twists-on-projective-space.md), take $S=k[X_0,\ldots,X_r]$ with the usual grading and $U_i=D_+(X_i)$. On an intersection indexed by the nonempty set $J$,

$$
\Gamma(U_J,\mathcal O(n))=\bigl(S[X_j^{-1}:j\in J]\bigr)_n.
$$

This follows directly from the construction of the [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md): sections of the twist are the degree-$n$ homogeneous fractions in the corresponding [localization](../../../../../localization-of-a-ring.md). The [Čech differential](../../../../../cech-differential.md) preserves each [Laurent monomial](../../../../../laurent-monomial.md) $X^a=X_0^{a_0}\cdots X_r^{a_r}$, where $a_i\in\mathbb Z$ and $\sum_i a_i=n$. Such a monomial appears precisely in summands with

$$
N(a):=\{i:a_i<0\}\subseteq J.
$$

The complex therefore decomposes as the direct sum of finite-dimensional [cochain complexes](../../../../../cochain-complex.md) indexed by these exponent vectors. Their differentials have only the alternating signs of the simplex incidence maps.

If $N(a)=\varnothing$, this is the ordinary unaugmented [simplex](../../../../../simplex.md) cochain complex: its degree-zero kernel consists of the common value on every vertex and has dimension one, while all higher cohomology vanishes. If $\varnothing\ne N(a)\ne\{0,\ldots,r\}$, choose $v\notin N(a)$. A [cochain homotopy](../../../../../cochain-homotopy.md) inserting $v$ into the ordered index list, with the sign of that insertion, contracts this subcomplex. Insertion or deletion of $v$ preserves the condition $N(a)\subseteq J$; in $\delta h+h\delta$, terms inserting and deleting different vertices cancel in pairs, while the term inserting then deleting $v$ is the identity. Thus this entire monomial subcomplex is acyclic. Finally, if all $a_i<0$, the monomial occurs only in the full intersection, in degree $r$, and contributes one copy of $k$ there.

For $r\ge1$, these three cases give the complete answer:

$$
\boxed{H^i(\mathbf P_k^r,\mathcal O(n))\cong
\begin{cases}
S_n,&i=0,\ n\ge0,\\
\displaystyle\bigoplus_{\substack{a_0,\ldots,a_r<0\\a_0+\cdots+a_r=n}}k\,X_0^{a_0}\cdots X_r^{a_r},&i=r,\ n\le-r-1,\\
0,&\text{otherwise}.
\end{cases}}
$$

In the first case counting nonnegative exponent vectors gives $h^0=\binom{n+r}{r}$. In the top case write $a_i=-1-b_i$ with $b_i\ge0$; then $\sum b_i=-n-r-1$, giving

$$
\boxed{h^r(\mathbf P_k^r,\mathcal O(n))=\binom{-n-1}{r}\quad(n\le-r-1).}
$$

This is the [Laurent-monomial description of top cohomology on projective space](../../../../../laurent-monomial-description-of-top-cohomology-on-projective-space.md). All intermediate degrees vanish for every twist, and the top degree vanishes when $n\ge-r$. If $r=0$, then $\mathbf P_k^0=\operatorname{Spec}k$ and every twist is trivial, so **$H^0(\mathbf P_k^0,\mathcal O(n))=k$ for every integer $n$, with all higher groups zero**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
