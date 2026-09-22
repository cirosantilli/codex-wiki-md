<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\mathcal A^{p,q}$ denote the [sheaf of differential forms of type (p, q)](../../../../../sheaf-of-differential-forms-of-type-p-q.md) printed in the PDF. Take the pointwise [Hermitian inner product](../../../../../hermitian-form.md) to be linear in its first argument, and use $\mathrm{vol}=\omega^n/n!$. The bidegrees in the question specify the [conjugate-linear Hodge star](../../../../../conjugate-linear-hodge-star.md): it is uniquely characterized by

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,\mathrm{vol},
\qquad \alpha,\beta\in\mathcal A^{p,q}.
$$

Thus $*(c\beta)=\bar c*\beta$, and $*$ maps bidegree $(p,q)$ to $(n-p,n-q)$. If $S$ is the complex-linear extension of the real [Hodge star operator](../../../../../hodge-star-operator.md), then $*=S\circ\text{complex conjugation}$. The operator $S$ is real and $S^2=(-1)^{k(2n-k)}$ on degree $k=p+q$, so

$$
\boxed{**\psi=(-1)^{p+q}\psi.}
$$

Using the complex-linear star instead would give a different bidegree, $(n-q,n-p)$; keeping the convention explicit prevents that ambiguity.

The [Hermitian Lefschetz operator](../../../../../lefschetz-operator-on-a-hermitian-manifold.md) is exterior multiplication by $\omega$. Define $\Lambda$ pointwise by

$$
\langle L\alpha,\beta\rangle=\langle\alpha,\Lambda\beta\rangle.
$$

It lowers bidegree by $(1,1)$. In a unitary real coframe with $\omega=\sum_j e^j\wedge f^j$, it is $\Lambda=\sum_j\iota_{f_j}\iota_{e_j}$, the corresponding sum of [interior product of a differential form](../../../../../interior-product.md) operators. This gives its existence and identifies it as a smooth operator. On a compact manifold, integrate the pointwise equality against $\mathrm{vol}$ to obtain

$$
(L\alpha,\beta)_{L^2}=(\alpha,\Lambda\beta)_{L^2}.
$$

No integration by parts is needed for this order-zero operator. Thus $\Lambda$ is both the pointwise and the global [formal adjoint](../../../../../formal-adjoint.md).

Write $[A,B]=AB-BA$, and let $k$ denote the degree of the input form. The given [Lefschetz commutator](../../../../../lefschetz-commutator.md) is $[L,\Lambda]=(k-n)I$. For $r=1$ the required formula is exactly this identity. If it holds for $r$, the [commutator derivation identity](../../../../../commutator-derivation-identity.md) gives

$$
[L^{r+1},\Lambda]=L[L^r,\Lambda]+[L,\Lambda]L^r.
$$

The second commutator acts on degree $k+2r$, so the coefficient on the right is

$$
r(k-n)+r(r-1)+(k+2r-n)
=(r+1)(k-n)+(r+1)r.
$$

This proves the [commutator formula for powers of the Lefschetz operator](../../../../../commutator-formula-for-powers-of-the-lefschetz-operator.md)

$$
\boxed{[L^r,\Lambda]=r(k-n+r-1)L^{r-1}.}
$$

For [injectivity of powers of the Lefschetz operator](../../../../../injectivity-of-powers-of-the-lefschetz-operator.md), $r=0$ is immediate. Suppose $r\ge1$ and $r+k\le n$. If $k=0$ or $1$, then $\Lambda\psi=0$, and $L^r\psi=0$ implies

$$
r(k-n+r-1)L^{r-1}\psi=0.
$$

The scalar is nonzero, since $k+r\le n$ makes $k-n+r-1\le-1$. Repeating with the smaller power shows $\psi=0$. For $k\ge2$, induct on $r+k$, treating all $r=0$ cases as already established. The same commutator calculation yields, with $c=r(k-n+r-1)\ne0$,

$$
L^{r-1}(L\Lambda\psi-c\psi)=0.
$$

The induction hypothesis applies to $L^{r-1}$ on degree $k$, since $(r-1)+k<r+k$ and $(r-1)+k\le n$. Hence $\psi=L\alpha$ with $\alpha=c^{-1}\Lambda\psi$ of degree $k-2$. Moreover $L^{r+1}\alpha=L^r\psi=0$. Since $(r+1)+(k-2)=r+k-1$, induction also makes $L^{r+1}$ injective on that degree, so $\alpha=0$ and $\psi=0$. All operators preserve restriction to open sets; the argument applies on every open set. Therefore **$L^r$ is an injective morphism of sheaves whenever $r+k\le n$**.

On a [Kähler manifold](../../../../../kahler-manifold.md), the [Kähler identities](../../../../../kahler-identities.md), with the positive form convention used above, are

$$
[\Lambda,\bar\partial]=-i\partial^*,\qquad
[\Lambda,\partial]=i\bar\partial^*.
$$

Taking [formal adjoints](../../../../../formal-adjoint.md) conjugates the scalar and reverses the order in the commutator. Since $\Lambda^*=L$, this gives

$$
\boxed{[L,\bar\partial^*]=-i\partial,\qquad
[L,\partial^*]=i\bar\partial.}
$$

To derive the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md), put $P=\partial$ and $B=\bar\partial$, so $P^2=B^2=0$ and $PB+BP=0$. Write $\{A,B\}=AB+BA$ for an [anticommutator](../../../../../anticommutator.md). The [Kähler identities](../../../../../kahler-identities.md) say $B^*=-i[\Lambda,P]$ and $P^*=i[\Lambda,B]$. Therefore

$$
\{P,B^*\}=-i\{P,[\Lambda,P]\}=0,\qquad
\{B,P^*\}=i\{B,[\Lambda,B]\}=0,
$$

because expansion leaves only terms containing $P^2$ or $B^2$. Furthermore,

$$
\begin{aligned}
\Delta_\partial&=i\{P,[\Lambda,B]\},\\
\Delta_{\bar\partial}&=-i\{B,[\Lambda,P]\}.
\end{aligned}
$$

Expanding these expressions and using $PB=-BP$ makes them equal. Since $d=P+B$ and $d^*=P^*+B^*$, the mixed [anticommutators](../../../../../anticommutator.md) already vanish, and consequently

$$
\boxed{\Delta_d=2\Delta_\partial=2\Delta_{\bar\partial}.}
$$

Closedness of the [Kähler form](../../../../../kahler-form.md) implies $[L,P]=[L,B]=0$. Using the adjoint identity above,

$$
[L,\Delta_{\bar\partial}]
=B[L,B^*]+[L,B^*]B
=-i(BP+PB)=0.
$$

The equality of the three [Laplacians](../../../../../laplacian.md) therefore proves **each Laplacian commutes with $L$**.

For a compact [Kähler manifold](../../../../../kahler-manifold.md), the [Dolbeault Hodge decomposition](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) is the orthogonal decomposition

$$
\mathcal A^{p,q}(M)=
\mathcal H^{p,q}\oplus
\operatorname{im}\bar\partial\oplus
\operatorname{im}\bar\partial^*.
$$

Here harmonicity for the [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) and for the [Hodge Laplacian](../../../../../hodge-laplacian.md) agrees by the preceding identity. If $\bar\partial\alpha=0$ and $\alpha=h+\bar\partial u+\bar\partial^*v$, then $\bar\partial\bar\partial^*v=0$. Taking its inner product with $v$ gives $\|\bar\partial^*v\|^2=0$. Thus $\alpha$ is cohomologous to $h$. Conversely, a harmonic form is $\bar\partial$-closed, and a harmonic exact form $h=\bar\partial u$ satisfies $\|h\|^2=(\bar\partial^*h,u)=0$. This proves existence and uniqueness of the harmonic representative and hence

$$
\boxed{H_{\bar\partial}^{p,q}(M)\cong\mathcal H^{p,q}(M).}
$$

These spaces are finite dimensional by the ellipticity of the [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) on the compact manifold.

Complex conjugation commutes with the real operator $\Delta_d$ and interchanges the bidegrees $(p,q)$ and $(q,p)$. It is therefore a conjugate-linear bijection of the harmonic spaces, proving [Hodge symmetry](../../../../../hodge-symmetry.md). The real [Hodge star operator](../../../../../hodge-star-operator.md) commutes with $\Delta_d$, as does complex conjugation; hence their composition, our [conjugate-linear Hodge star](../../../../../conjugate-linear-hodge-star.md), sends harmonic $(p,q)$-forms bijectively to harmonic $(n-p,n-q)$-forms. Its square is the nonzero scalar established above. This proves [Hodge duality](../../../../../hodge-duality.md), and gives

$$
\boxed{h^{p,q}=h^{q,p},\qquad h^{p,q}=h^{n-p,n-q}.}
$$

For the final [hard Lefschetz isomorphism on Dolbeault cohomology](../../../../../hard-lefschetz-isomorphism-on-dolbeault-cohomology.md), take $k=p+q\le n$ and $r=n-k$. This restriction is necessary to make the displayed power nonnegative. The [Hermitian Lefschetz operator](../../../../../lefschetz-operator-on-a-hermitian-manifold.md) raises bidegree by $(1,1)$, and the [Lefschetz operator preserves harmonic forms](../../../../../lefschetz-operator-preserves-harmonic-forms.md); therefore

$$
L^{n-k}:\mathcal H^{p,q}\longrightarrow
\mathcal H^{n-q,n-p}
$$

is well defined. It is injective by [injectivity of powers of the Lefschetz operator](../../../../../injectivity-of-powers-of-the-lefschetz-operator.md), since $r+k=n$. [Hodge symmetry](../../../../../hodge-symmetry.md) and [Hodge duality](../../../../../hodge-duality.md) give $h^{n-q,n-p}=h^{q,p}=h^{p,q}$, so it is a bijection between finite-dimensional spaces of equal dimension. Because $[L,\bar\partial]=0$, the map on harmonic representatives agrees with exterior multiplication by $[\omega]^{n-k}$ on [Dolbeault cohomology](../../../../../dolbeault-cohomology.md). We conclude

$$
\boxed{L^{n-p-q}:H_{\bar\partial}^{p,q}(M)
\xrightarrow{\ \cong\ }H_{\bar\partial}^{n-q,n-p}(M),
\qquad p+q\le n.}
$$

For $p+q>n$, the corresponding valid statement is the inverse of the positive-power isomorphism from bidegree $(n-q,n-p)$ to $(p,q)$; a negative exterior-multiplication power is not defined.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
