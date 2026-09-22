<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [unnormalized parabolic induction](../../../../../../unnormalized-parabolic-induction.md), the convention fixed by the supplied sequence and by the occurrence of constants in $V(1)$. Its functions satisfy $f(bg)=\chi(b)f(g)$, and $G$ acts by right translation. Characters in this smooth category are [smooth characters](../../../../../../smooth-character.md). Put $\lambda=\chi^w\delta^{-1}$, retaining the question's modulus $\delta(\operatorname{diag}(a,d))=|d/a|$.

First derive the [evaluation adjunction for unnormalized induction](../../../../../../evaluation-adjunction-for-unnormalized-induction.md). A $G$-intertwiner $A:V(\chi)\to V(\xi)$ gives a functional $\ell(v)=A(v)(1)$. Since $A$ intertwines and induced functions have left covariance, $\ell(\pi(b)v)=\xi(b)\ell(v)$. Conversely such a functional defines

$$
A(v)(g)=\ell(\pi(g)v).
$$

This function has the required left covariance. Any [compact-open subgroup](../../../../../../compact-open-subgroup.md) fixing $v$ fixes it on the right, so it is a smooth induced function; compactness of $B\backslash G$ removes any additional support issue. The construction is $G$-equivariant, and the two operations are inverse. Since $\xi$ is trivial on $U$, these functionals factor precisely through the [Jacquet module](../../../../../../jacquet-module.md), giving

$$
\operatorname{Hom}_G(V(\chi),V(\xi))\cong\operatorname{Hom}_T(V(\chi)_U,\xi).
$$

Now use the given exact sequence $0\to\lambda\to J\to\chi\to0$, where $J=V(\chi)_U$ has dimension two.

If $\lambda\ne\chi$, choose $t_0\in T$ on which their values differ. Its operator on $J$ is upper triangular with distinct [eigenvalues](../../../../../../eigenvalue.md), so has two one-dimensional [eigenspaces](../../../../../../eigenspace.md). Since $T$ is abelian, all its operators commute with this operator and preserve the [eigenspaces](../../../../../../eigenspace.md). They are the [linear character](../../../../../../linear-character.md) lines $\lambda$ and $\chi$. This proves that [distinct-character extensions of an abelian group split](../../../../../../distinct-character-extensions-of-an-abelian-group-split.md), so $J\cong\lambda\oplus\chi$. A map between one-dimensional [linear character](../../../../../../linear-character.md) spaces is zero unless the [linear characters](../../../../../../linear-character.md) agree, and otherwise is one-dimensional. Therefore the required dimension is one for $\xi=\lambda$ or $\xi=\chi$, and zero for any other [linear character](../../../../../../linear-character.md).

The case $\lambda=\chi$ needs an extra argument: the exact sequence alone would also permit a split self-extension with two quotient functionals. Write $\chi(\operatorname{diag}(a,d))=\chi_1(a)\chi_2(d)$. Equality with $\lambda$ forces $\chi_1/\chi_2=|\cdot|$, so $\chi=(\eta\circ\det)\chi_0$, where $\eta=\chi_2$ and $\chi_0(\operatorname{diag}(a,d))=|a|$. Multiplication of induced functions by $\eta(\det g)$ identifies this with a determinant-character twist of $V(\chi_0)$. Twisting is invertible, so it is enough to prove nonsplitting for $\chi_0$.

Use the open [Bruhat decomposition](../../../../../../bruhat-decomposition.md) coordinate

$$
w=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad n(x)=\begin{pmatrix}1&x\\0&1\end{pmatrix},\qquad g_f(x)=f(wn(x)),\quad x\in F.
$$

For $x\ne0$ the matrix factorization

$$
wn(x)=\begin{pmatrix}x^{-1}&-1\\0&x\end{pmatrix}\begin{pmatrix}1&0\\x^{-1}&1\end{pmatrix}
$$

shows that $g_f(x)=|x|^{-1}f(1)$ for all sufficiently large $|x|$: the lower-unipotent matrix approaches the identity, where $f$ is locally constant. The coordinate map is injective, since this open cell is dense in the projective-line quotient and induced functions are locally constant sections.

For $t=\operatorname{diag}(a,d)$, direct multiplication gives

$$
g_{\pi(t)f}(x)=|d|g_f((d/a)x).
$$

There exists a section $f_0$ with $f_0(1)=1$ and coordinate function

$$
g_0(x)=\begin{cases}1,&|x|\le1,\\|x|^{-1},&|x|>1.\end{cases}
$$

Indeed the displayed factorization changes to the lower chart near infinity, where this tail corresponds to the constant function one. Thus it extends smoothly across the missing point. With $t=\operatorname{diag}(\varpi,1)$ and $|\varpi|=q^{-1}$, the difference is the compactly supported function

$$
h(x)=g_0(x/\varpi)-q^{-1}g_0(x)=(1-q^{-1})1_{\varpi\mathfrak o}(x).
$$

Normalize additive [Haar measure](../../../../../../haar-measure.md) by $\operatorname{vol}(\mathfrak o)=1$. Then

$$
\int_Fh(x)dx=(1-q^{-1})q^{-1}\ne0.
$$

This difference survives in the [Jacquet module](../../../../../../jacquet-module.md). To prove that assertion, the unipotent action translates coordinates: $g_{\pi(n(y))f}(x)=g_f(x+y)$. Any such translation difference is compactly supported because the tail is $f(1)|x|^{-1}$ and $|x+y|=|x|$ when $|x|$ is sufficiently large. Its integral is zero: integrate over a sufficiently large additive ball, invariant under translation by $y$, and change variables. A finite sum of unipotent translation differences also has integral zero. Hence $h$, whose integral is nonzero, cannot be a coinvariant relation. In particular, on $J$ the operator $\pi(t)-\chi_0(t)I$ is nonzero. This proves the [equal-character Jacquet self-extension for GL2](../../../../../../equal-character-jacquet-self-extension-for-gl2.md) is nonsplit.

Any $T$-equivariant functional $J\to\chi_0$ must kill the nonzero image of that operator. Since $J$ has dimension two, its space of such functionals has dimension at most one; the quotient in the supplied exact sequence already provides one. Twisting back gives the same conclusion for the common [linear character](../../../../../../linear-character.md) $\chi=\lambda$. For any different $\xi$, a surjection $J\to\xi$ is impossible because both composition factors of $J$ are $\chi$. Combining the two cases gives

$$
\boxed{\dim\operatorname{Hom}_G(V(\chi),V(\xi))=\begin{cases}1,&\xi=\chi\text{ or }\xi=\chi^w\delta^{-1},\\0,&\text{otherwise}.\end{cases}}
$$

When the two listed [linear characters](../../../../../../linear-character.md) coincide, the dimension remains one; they are not two independent contributions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
