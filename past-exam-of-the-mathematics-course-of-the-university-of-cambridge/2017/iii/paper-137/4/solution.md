<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First establish [rational conjugation of finite-index modular subgroups](../../../../../rational-conjugation-of-finite-index-modular-subgroups.md) without assuming that $\Gamma$ is a [congruence subgroup](../../../../../congruence-subgroup.md). Multiply $\gamma$ by a positive integer to obtain an integral [matrix](../../../../../matrix.md) $A$, and let $D=\det A>0$. Conjugation is unchanged by this scalar. If $h=I+DB\in\Gamma(D)$, then

$$
AhA^{-1}=I+AB\operatorname{adj}(A)\in SL_2(\mathbb Z).
$$

Thus the [principal congruence subgroup](../../../../../principal-congruence-subgroup.md) $\Gamma(D)$ is contained in $H=SL_2(\mathbb Z)\cap\gamma^{-1}SL_2(\mathbb Z)\gamma$. It has finite index because reduction modulo $D$ has finite image. Inside $H$, pullback under conjugation of $\Gamma$ has relative index at most $[SL_2(\mathbb Z):\Gamma]$. Consequently

$$
\boxed{[SL_2(\mathbb Z):\Gamma']<\infty,
\quad\Gamma'=SL_2(\mathbb Z)\cap\gamma^{-1}\Gamma\gamma.}
$$

This argument does not assert that an arbitrary [finite-index subgroup](../../../../../finite-index-subgroup.md) contains a [principal congruence subgroup](../../../../../principal-congruence-subgroup.md).

Use the [determinant-normalized slash operator](../../../../../determinant-normalized-slash-operator.md)

$$
(f|_k\gamma)(z)=(\det\gamma)^{k/2}(cz+d)^{-k}f\left(\frac{az+b}{cz+d}\right),
\quad\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix},\quad\det\gamma>0.
$$

The positive real power of the [determinant](../../../../../determinant.md) is used; on $SL_2(\mathbb Z)$ this reduces to the usual [slash operator for modular forms](../../../../../slash-operator-for-modular-forms.md). The [automorphy factor](../../../../../automorphy-factor.md) identity gives the right-action rule $(f|_k\gamma)|_k\eta=f|_k(\gamma\eta)$.

A [modular form on a finite-index subgroup](../../../../../modular-form-on-a-finite-index-subgroup.md) of integer weight $k$ is a [holomorphic function](../../../../../holomorphic-function.md) on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), invariant under this weight-$k$ action of $\Gamma$, and [holomorphic at a cusp](../../../../../holomorphic-at-a-cusp.md) at each of its cusps. A [cusp of a modular group](../../../../../cusp-of-a-modular-group.md) is a $\Gamma$ orbit in $\mathbb P^1(\mathbb Q)$. If $\sigma\in SL_2(\mathbb Z)$ carries infinity to its representative, choose a positive integer $h$ with $\sigma T^h\sigma^{-1}\in\Gamma$. Such $h$ exists by finite index. Then $f|_k\sigma$ is periodic and has a convergent expansion in $q_h=e^{2\pi iz/h}$ near zero; holomorphy means no negative exponents, and being a [cusp form](../../../../../cusp-form.md) means zero constant term. Using an actual translation period avoids possible signs if a smaller [width of a cusp](../../../../../width-of-a-cusp.md) is defined only modulo the center, particularly in odd weights.

For [cusp holomorphy under rational slash operators](../../../../../cusp-holomorphy-under-rational-slash-operators.md), choose $\sigma\in SL_2(\mathbb Z)$ with $\sigma\infty=\gamma\infty$, possible by completing a primitive integer pair to a determinant-one [matrix](../../../../../matrix.md). Then $\sigma^{-1}\gamma=\begin{pmatrix}a&b\\0&d\end{pmatrix}$, with $a/d>0$. Up to a nonzero constant factor,

$$
f|_k\gamma(z)=(f|_k\sigma)((a/d)z+b/d).
$$

The imaginary part of the argument tends to infinity with that of $z$, so this remains bounded by the cusp expansion of $f|_k\sigma$. It tends to zero if $f$ is a [cusp form](../../../../../cusp-form.md). Moreover $f|_k\gamma$ is invariant under $\Gamma'$: for $\eta\in\Gamma'$, $\gamma\eta\gamma^{-1}\in\Gamma$ and the right-action rule applies. Finite index gives a translation period for $\Gamma'$, so boundedness is a [removable singularity](../../../../../removable-singularity.md) at zero in that periodic parameter. This proves holomorphy at infinity. For every other cusp, apply the same argument to the rational [matrix](../../../../../matrix.md) $\gamma\rho$, with $\rho\in SL_2(\mathbb Z)$. Thus all cusp conditions hold, and

$$
\boxed{f|_k\gamma\in M_k(\Gamma').}
$$

For the [character twist by rational translations of a cusp form](../../../../../character-twist-by-rational-translations-of-a-cusp-form.md), put $B_j=\begin{pmatrix}1&j/N\\0&1\end{pmatrix}$ and $K=\Gamma_1(N)\cap\Gamma_0(N^2)$. For $\eta=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in K$, direct conjugation gives

$$
B_j\eta B_j^{-1}=\begin{pmatrix}
a+jc/N&b+j(d-a)/N-j^2c/N^2\\
c&d-jc/N
\end{pmatrix}\in SL_2(\mathbb Z).
$$

Indeed $N^2\mid c$ and $a\equiv d\equiv1\pmod N$. Every $f|_kB_j=f(z+j/N)$ is therefore $K$-invariant and vanishes at all its cusps by the preceding rational-translate argument. Their finite weighted sum is a [cusp form](../../../../../cusp-form.md), for every [Dirichlet character](../../../../../dirichlet-character.md):

$$
\boxed{f_\chi\in S_k(\Gamma_1(N)\cap\Gamma_0(N^2)).}
$$

There is, however, **a missing primitivity hypothesis in the printed final expansion claim**. The exact [Fourier expansion of a modular form](../../../../../fourier-expansion-of-a-modular-form.md) is always

$$
\boxed{f_\chi(z)=\sum_{n\geq1}a_n(f)S_{\overline\chi}(n)q^n,
\quad S_{\overline\chi}(n)=\sum_{j\in(\mathbb Z/N\mathbb Z)^\times}\overline{\chi(j)}e^{2\pi inj/N}.}
$$

Values of a [Dirichlet character](../../../../../dirichlet-character.md) on units have modulus one, so $\chi(j)^{-1}=\overline{\chi(j)}$. For unit $n$, substitution gives $S_{\overline\chi}(n)=\chi(n)g(\overline\chi)$, where $g$ is the [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md). For nonunit $n$, this vanishing formula requires a [primitive Dirichlet character](../../../../../primitive-dirichlet-character.md).

Here is its proof in that case. Choose a [prime](../../../../../prime-number.md) $p\mid(n,N)$. Primitivity supplies a unit $u\equiv1\pmod{N/p}$ with $\chi(u)\ne1$: otherwise the character would factor through the surjective reduction to units modulo $N/p$. Surjectivity follows by lifting a unit and, if needed, adjusting the lift to avoid the additional prime $p$, using the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md). Multiplication by $u$ fixes $e^{2\pi inj/N}$ because $p\mid n$, but multiplies the character factor by a nontrivial constant. Hence $S_{\overline\chi}(n)=0$. The [finite Fourier transform of a primitive Dirichlet character](../../../../../finite-fourier-transform-of-a-primitive-dirichlet-character.md) now gives the corrected formula

$$
\boxed{f_\chi=g(\overline\chi)\sum_{n\geq1}\chi(n)a_n(f)q^n
\quad\text{if }\chi\text{ is primitive modulo }N.}
$$

The constant is nonzero: finite exponential orthogonality gives $\sum_{n\bmod N}|S_{\overline\chi}(n)|^2=N\varphi(N)$, whereas the proved formula makes this $\varphi(N)|g(\overline\chi)|^2$. Thus $|g(\overline\chi)|=\sqrt N$.

For a concrete counterexample to the printed unrestricted claim, take $N=2$, the [principal Dirichlet character](../../../../../principal-dirichlet-character.md), and $f=\Delta$. The translation sum is $\Delta(z+1/2)=\sum_n(-1)^n\tau(n)q^n$, whose $q^2$ coefficient is $-24$. Any constant multiple of the proposed odd-index-only series has $q^2$ coefficient zero. Thus the general modularity conclusion is proved, while the claimed simplification is false without the stated extra hypothesis.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
