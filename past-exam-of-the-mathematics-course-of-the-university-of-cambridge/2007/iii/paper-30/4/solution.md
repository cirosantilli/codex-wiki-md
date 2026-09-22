<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $d=\gcd(k,p-1)$ and write $S(a)=\sum_{x\in\mathbb F_p}e(ax^k/p)=pG_{a,p}$. The [multiplicative group of a finite field is cyclic](../../../../../multiplicative-group-of-a-finite-field-is-cyclic.md), so on its nonzero elements the $k$th-power map has kernel of size $d$. For $y\ne0$, [character orthogonality](../../../../../character-orthogonality.md) consequently gives

$$
\#\{x:x^k=y\}=\sum_{\chi^d=1}\chi(y),
$$

where the sum is over its multiplicative [characters](../../../../../character-of-a-representation.md). Thus, for $a\ne0$,

$$
S(a)=1+\sum_{\chi^d=1}\sum_{y\ne0}\chi(y)e(ay/p)=\sum_{\substack{\chi^d=1\\\chi\ne1}}\tau(\chi,a).
$$

The term from the trivial [character](../../../../../character-of-a-representation.md) is $-1$ and cancels the initial one.

For a nontrivial [character](../../../../../character-of-a-representation.md), the [prime-field character Gauss sum identity](../../../../../prime-field-character-gauss-sum-identity.md) can be proved directly. Since $|\chi(z)|=1$ on nonzero elements, substituting $y=tz$ gives

$$
|\tau(\chi,a)|^2=\sum_{t\ne0}\chi(t)\sum_{z\ne0}e(a(t-1)z/p).
$$

The inner sum is $p-1$ for $t=1$ and $-1$ otherwise. Since $\sum_{t\ne0}\chi(t)=0$, the result is $p$. The [triangle inequality](../../../../../triangle-inequality.md) now proves the [power Gauss sum over a prime field](../../../../../power-gauss-sum-over-a-prime-field.md) bound

$$
\boxed{|G_{a,p}|\le\frac{d-1}{\sqrt p}\le\frac k{\sqrt p}.}
$$

This also includes $d=1$, when the nonzero-frequency sum vanishes.

For $x\in\mathbb F_p$, additive [character orthogonality](../../../../../character-orthogonality.md) counts its representations as three powers:

$$
R(x)=\#\{(u,v,w):u^k+v^k+w^k=x\}=\frac1p\sum_{a\in\mathbb F_p}S(a)^3e(-ax/p).
$$

The zero-frequency term is $p^2$. Each other term has $|S(a)|\le k\sqrt p$, so

$$
|R(x)-p^2|\le\frac{p-1}{p}k^3p^{3/2}<k^3p^{3/2}.
$$

If $p>k^6$, this is less than $p^2$, giving $R(x)>0$ for every $x$. Hence **$p>k^6$ is a sufficient threshold** for the [three power summands over a large prime field](../../../../../three-power-summands-over-a-large-prime-field.md) conclusion.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
