<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $A,B$ for the two given [congruence subgroups](../../../../../congruence-subgroup.md), to distinguish them from the notation $\Gamma_1(N)$. Their [double coset](../../../../../double-coset.md) has a finite decomposition

$$
A\alpha B=\coprod_{j=1}^r A\alpha_j.
$$

Finiteness follows because $B\cap\alpha^{-1}A\alpha$ has finite index in $B$. To check this without assuming integrality of $\alpha$, clear its denominators: a sufficiently deep [principal congruence subgroup](../../../../../principal-congruence-subgroup.md) lies both in $B$ and, after conjugation by $\alpha$, in $A$. Representatives for $(B\cap\alpha^{-1}A\alpha)\backslash B$ give the displayed decomposition.

Using the [Hecke-normalized rational slash operator](../../../../../hecke-normalized-rational-slash-operator.md) from the PDF, define the [double-coset operator on modular forms](../../../../../double-coset-operator-on-modular-forms.md) by

$$
\boxed{[A\alpha B]f=\sum_{j=1}^r f[\alpha_j]_k.}
$$

Replacing $\alpha_j$ by $\gamma\alpha_j$ for $\gamma\in A$ changes no term because $f[\gamma]_k=f$. Right multiplication by $\beta\in B$ permutes these left cosets, so $([A\alpha B]f)[\beta]_k=[A\alpha B]f$. Each summand is holomorphic in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). At any rational [modular cusp](../../../../../cusp-of-a-modular-group.md), factor $\alpha_j\rho=\sigma C$ with $\sigma\in SL_2(\mathbb Z)$ and $C$ upper triangular of positive slope, as in 2(i). The cusp expansion of $f[\sigma]_k$ has no negative terms, and substitution by $C$ preserves boundedness. The sum is periodic in a cusp coordinate for $B$, so it has a removable singularity there. This proves

$$
\boxed{[A\alpha B]f\in M_k(B).}
$$

If $f$ vanishes at all its cusps, the same argument gives vanishing for the image too.

Now set $\Gamma=\Gamma_1(N)$. For an integer $d$ prime to $N$, choose $\sigma_d\in\Gamma_0(N)$ with lower-right entry congruent to $d$ modulo $N$. Such a lift exists by choosing $a$ with $ad\equiv1\pmod N$ and using $\begin{pmatrix}a&(ad-1)/N\\N&d\end{pmatrix}$. The subgroup $\Gamma$ is normal in $\Gamma_0(N)$, and its quotient is $(\mathbb Z/N\mathbb Z)^\times$ through the lower-right entry. Define the [diamond operator](../../../../../diamond-operator.md) by

$$
\boxed{\langle d\rangle f=f[\sigma_d]_k.}
$$

Different lifts differ by a member of $\Gamma$, so this is well defined. The [diamond operators](../../../../../diamond-operator.md) satisfy $\langle d\rangle\langle e\rangle=\langle de\rangle$.

For a prime $p\nmid N$, put $A_p=\operatorname{diag}(1,p)$ and define the [Hecke operator](../../../../../hecke-operator.md)

$$
\boxed{T_p=[\Gamma A_p\Gamma].}
$$

Choose $a,b\in\mathbb Z$ with $ap-bN=1$ and set $\sigma_p=\begin{pmatrix}a&b\\N&p\end{pmatrix}$. A complete set of left-coset representatives is

$$
A_j=\begin{pmatrix}1&j\\0&p\end{pmatrix}\quad(0\leq j<p),\qquad B_p=\sigma_p\begin{pmatrix}p&0\\0&1\end{pmatrix}.
$$

Here $A_j=A_pT^j$ and $B_p=A_p\begin{pmatrix}ap&b\\N&1\end{pmatrix}$, with both right factors in $\Gamma$. To prove completeness, $H=\Gamma\cap A_p^{-1}\Gamma A_p$ consists of the members of $\Gamma$ whose upper-right entry is divisible by $p$. Reduction of $\Gamma$ modulo $p$ is onto $SL_2(\mathbb F_p)$: use the Chinese remainder theorem to impose identity modulo $N$ and any chosen determinant-one matrix modulo $p$, then lift to $SL_2(\mathbb Z)$ by elementary matrices. Reduction of $H$ is the lower triangular subgroup. Its left cosets correspond to the $p+1$ lines of top rows in $\mathbb F_p^2$. The right factors $T^j$ give lines $[1:j]$, while the last factor gives $[0:b]$ with $b\not\equiv0\pmod p$. They are all the lines, proving the decomposition.

The printed slash normalization now gives $f[A_j]_k=p^{-1}f((\tau+j)/p)$ and

$$
f[B_p]_k=(\langle p\rangle f)\left[\begin{pmatrix}p&0\\0&1\end{pmatrix}\right]_k
=p^{k-1}(\langle p\rangle f)(p\tau).
$$

Thus

$$
\boxed{T_pf=\frac1p\sum_{j=0}^{p-1}f\left(\frac{\tau+j}{p}\right)+p^{k-1}(\langle p\rangle f)(p\tau).}
$$

To prove commutation, use the [marked-lattice model of a modular form](../../../../../marked-lattice-model-of-a-modular-form.md). A pair $(L,t)$ consists of a lattice and a point of exact order $N$ modulo $L$, and a weight-$k$ function satisfies $F(uL,ut)=u^{-k}F(L,t)$. In a basis $L=\mathbb Z\tau+\mathbb Z$ with $t=1/N$, it represents $f(\tau)$. The [diamond operator](../../../../../diamond-operator.md) multiplies $t$ by $d$. The same [Hecke operator](../../../../../hecke-operator.md) is

$$
T_pF(L,t)=\frac1p\sum_{L'\supset L\,;\,[L':L]=p}F(L',t\bmod L').
$$

Every marked point retains exact order $N$: multiplication by $p$ is invertible on its cyclic group, since $p\nmid N$. This lattice sum agrees with the displayed slash sum. Its $p$ overlattices with basis $((\tau+j)/p,1)$ give the first terms, and the remaining one with basis $(\tau,1/p)$ has normalized marked point $p/N$, giving $p^{k-1}(\langle p\rangle f)(p\tau)$. Multiplying the mark by $d$ commutes with passage to each overlattice and does not change the set of overlattices. Hence

$$
\boxed{\langle d\rangle T_p=T_p\langle d\rangle.}
$$

Finally write $f=\sum_{m\geq0}a_m(f)q^m$. The first term of $T_p$ contains the finite average

$$
\frac1p\sum_{j=0}^{p-1}e^{2\pi i mj/p}=\begin{cases}1&p\mid m,\\0&p\nmid m.\end{cases}
$$

It therefore contributes $a_{np}(f)$ to the coefficient of $q^n$. The second term contributes $p^{k-1}a_{n/p}(\langle p\rangle f)$ if $p\mid n$, and zero otherwise. This proves the [good-prime and bad-prime Hecke coefficient formula](../../../../../good-prime-and-bad-prime-hecke-coefficient-formula.md) at a good prime, without assuming that $f$ has a particular character:

$$
\boxed{a_n(T_pf)=a_{np}(f)+p^{k-1}a_{n/p}(\langle p\rangle f),}
$$

where a nonintegral coefficient index means zero. For $n=0$ both terms are retained. On a diamond-character eigenspace the second term becomes $\chi(p)p^{k-1}a_{n/p}(f)$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 88](../../paper-88-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
