<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write $U_u=\begin{pmatrix}1&u/D\\0&1\end{pmatrix}$ and $\tau(\chi)=\sum_{u\bmod D}\chi(u)e^{2\pi iu/D}$. The [finite Fourier transform of a primitive Dirichlet character](../../../../../finite-fourier-transform-of-a-primitive-dirichlet-character.md) gives

$$
\sum_{u\bmod D}\overline\chi(u)e^{2\pi inu/D}=\chi(n)\tau(\overline\chi).
$$

For $(n,D)=1$ this follows by multiplying residues by $n$. For a nonunit $n$, primitivity supplies a unit $v\equiv1\pmod{D/p}$ with nontrivial character value, for a prime $p\mid(n,D)$; multiplication by $v$ leaves the exponential unchanged and forces the sum to vanish. Orthogonality of the finite exponentials gives $\sum_{n\bmod D}|\sum_u\chi(u)e^{2\pi inu/D}|^2=D\sum_u|\chi(u)|^2=D\varphi(D)$. The primitive transform identity makes the left side $\varphi(D)|\tau(\chi)|^2$. Thus the primitive [Gauss sum of a Dirichlet character](../../../../../gauss-sum-of-a-dirichlet-character.md) is nonzero, with $|\tau(\chi)|^2=D$. Consequently the twist is the finite rational-translation sum

$$
\boxed{f_\chi=\frac1{\tau(\overline\chi)}\sum_{u\bmod D}\overline\chi(u)f|_kU_u.}
$$

This representation will prove both the level statement and the Fricke formula.

Take $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(ND^2)$, and choose $v\equiv d^2u\pmod D$. Since $ad\equiv1\pmod D$, this means $av\equiv ud\pmod D$. Direct multiplication gives

$$
U_u\gamma U_v^{-1}
=\begin{pmatrix}
a+uc/D&b+(ud-av)/D-ucv/D^2\\
c&d-cv/D
\end{pmatrix}=:\gamma_u.
$$

Every entry is integral, its [determinant](../../../../../determinant.md) is one, and its lower-left entry is divisible by $N$. Thus $\gamma_u\in\Gamma_0(N)$. Its lower-right entry is congruent to $d$ modulo $N$, so $f|\gamma_u=\psi(d)f$ by its [nebentypus character](../../../../../nebentypus-character.md). Using the right-action property of the slash operator,

$$
f_\chi|\gamma=\frac{\psi(d)}{\tau(\overline\chi)}
\sum_u\overline\chi(u)f|U_v.
$$

The map $u\mapsto v=d^2u$ permutes the residue classes. Reindexing gives $\overline\chi(u)=\chi(d)^2\overline\chi(v)$, so

$$
\boxed{f_\chi|_k\gamma=\psi(d)\chi(d)^2f_\chi.}
$$

This proves the required [modular weight](../../../../../weight-of-a-modular-form.md) and character on $\Gamma_0(ND^2)$.

Cuspidality must also be checked. For any [modular cusp](../../../../../cusp-of-a-modular-group.md) [matrix](../../../../../matrix.md) $\sigma\in SL_2(\mathbb Z)$ and any rational translation $U_u$, choose $\rho\in SL_2(\mathbb Z)$ with $\rho\infty=U_u\sigma\infty$. Then $\rho^{-1}U_u\sigma$ is upper triangular with positive dilation. Since $f|\rho$ decays exponentially at infinity, so does $f|U_u\sigma$. The finite sum defining $f_\chi$ therefore tends to zero at every [modular cusp](../../../../../cusp-of-a-modular-group.md); its transformation law supplies a [modular cusp](../../../../../cusp-of-a-modular-group.md) period, so its holomorphic [Fourier expansion](../../../../../fourier-series-split.md) has zero constant term there. Hence the [primitive twist at coprime level](../../../../../primitive-twist-at-coprime-level.md) is

$$
\boxed{f_\chi\in S_k(\Gamma_0(ND^2),\psi\chi^2).}
$$

Now put $W_M=\begin{pmatrix}0&-1\\M&0\end{pmatrix}$ and $g=f|_kW_N$, always using the [determinant](../../../../../determinant.md) factor specified in the question. For each unit $u$ choose a unit $v$ with $Nuv\equiv-1\pmod D$, possible because $(N,D)=1$. The crucial integral [matrix](../../../../../matrix.md) factorization is

$$
\boxed{U_uW_{ND^2}=D\gamma_uW_NU_v,\qquad
\gamma_u=\begin{pmatrix}(1+Nuv)/D&u\\Nv&D\end{pmatrix}\in\Gamma_0(N).}
$$

The right side multiplies out to $\begin{pmatrix}uND&-1\\ND^2&0\end{pmatrix}$, so the identity is exact. Its determinant-one [matrix](../../../../../matrix.md) has lower-right entry $D$, and therefore $f|\gamma_u=\psi(D)f$. A positive scalar [matrix](../../../../../matrix.md) $DI$ acts trivially under the [determinant-normalized slash operator](../../../../../determinant-normalized-slash-operator.md), since its [determinant](../../../../../determinant.md) contributes $D^k$ and its denominator contributes $D^{-k}$. Thus

$$
f_\chi|W_{ND^2}=\frac{\psi(D)}{\tau(\overline\chi)}\sum_u\overline\chi(u)g|U_v.
$$

The inverse-residue substitution is $u\equiv-(Nv)^{-1}\pmod D$, giving $\overline\chi(u)=\chi(-N)\chi(v)$. The sum over $v$ is $\tau(\chi)g_{\overline\chi}$. Hence the [Fricke transform of a primitive coprime twist](../../../../../fricke-transform-of-a-primitive-coprime-twist.md) is

$$
\boxed{f_\chi|_kW_{ND^2}=\psi(D)\chi(-N)\frac{\tau(\chi)}{\tau(\overline\chi)}\,g_{\overline\chi}
=\psi(D)\chi(N)\frac{\tau(\chi)^2}{D}\,g_{\overline\chi}.}
$$

The second version uses $\tau(\chi)\tau(\overline\chi)=\chi(-1)D$, which follows from $\overline{\tau(\chi)}=\chi(-1)\tau(\overline\chi)$ and $|\tau(\chi)|^2=D$. Here $g_{\overline\chi}=\sum b(n)\overline\chi(n)q^n$ if $g=\sum b(n)q^n$; it is not the complex conjugate function $\overline g$. The coprimality of $N,D$ is used both in the [matrix](../../../../../matrix.md) factorization and in evaluating $\psi(D)$. For $D=1$ the twist is trivial and the formula simply reads $f|W_N=g$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
