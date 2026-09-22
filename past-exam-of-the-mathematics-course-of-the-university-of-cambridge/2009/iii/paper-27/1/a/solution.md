<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [determinant-normalized slash operator](../../../../../../determinant-normalized-slash-operator.md) and the usual [Hecke operator](../../../../../../hecke-operator.md) normalization. A normalized eigenform is a nonzero [cusp form](../../../../../../cusp-form.md) $f=\sum_{r\ge1}a_rq^r$ with $a_1=1$ and $T_nf=\lambda(n)f$ for every $n$. We first establish the operator facts needed here, rather than assume the [Hecke multiplication relations](../../../../../../hecke-multiplication-relations.md).

Integer matrices of [determinant](../../../../../../determinant.md) $n$ have the [determinant-n matrix representatives for Hecke operators](../../../../../../determinant-n-matrix-representatives-for-hecke-operators.md) $\gamma_{a,b,d}=\left(\begin{smallmatrix}a&b\\0&d\end{smallmatrix}\right)$, with $ad=n$ and $0\le b<d$. Integer row operations give these representatives: the [Euclidean algorithm](../../../../../../euclidean-algorithm.md) reduces the first column to $(a,0)$, and a shear reduces $b$ modulo $d$. Right multiplication by the [modular group](../../../../../../modular-group.md) permutes the left cosets, so $T_nf=n^{k/2-1}\sum_{ad=n}\sum_{b\bmod d}f|_k\gamma_{a,b,d}$ is modular. Rational changes of coordinate preserve cusp vanishing, so it remains a [cusp form](../../../../../../cusp-form.md). Substituting its [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) and summing $e^{2\pi i rb/d}$ gives

$$
a_m(T_nf)=\sum_{d\mid\gcd(m,n)}d^{k-1}a_{mn/d^2}(f).
$$

In particular $a_1(T_nf)=a_n(f)$, and the normalization gives $\lambda(n)=a_n(f)$ for every $n$.

For coprime $u,v$, applying this coefficient formula twice amounts to choosing independently a divisor of $\gcd(m,u)$ and one of $\gcd(m,v)$. Their product runs exactly once through the divisors of $\gcd(m,uv)$, with the same factor $d^{k-1}$ and coefficient index. Thus $T_uT_v=T_{uv}$. For a prime $p$, put $P=p^{k-1}$ and $\nu=v_p(m)$. The coefficient of $q^m$ in $T_{p^e}f$ is

$$
A_e(m)=\sum_{j=0}^{\min(e,\nu)}P^j a_{p^em/p^{2j}}.
$$

The coefficient in $T_pT_{p^e}f$ is $A_e(pm)+P A_e(m/p)$, the second summand being zero if $p\nmid m$. Expanding the two finite sums and matching their endpoints gives $A_{e+1}(m)+P A_{e-1}(m)$ for $e\ge1$. Equality of all coefficients proves $T_pT_{p^e}=T_{p^{e+1}}+p^{k-1}T_{p^{e-1}}$. Applying these identities to the nonzero [eigenvector](../../../../../../eigenvector.md) $f$ yields

$$
\boxed{\lambda(uv)=\lambda(u)\lambda(v)\quad(\gcd(u,v)=1),\qquad
\lambda(p^{e+2})=\lambda(p)\lambda(p^{e+1})-p^{k-1}\lambda(p^e).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
