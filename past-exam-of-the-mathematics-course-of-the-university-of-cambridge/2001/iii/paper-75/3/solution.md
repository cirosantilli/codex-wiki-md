<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [determinant-normalized slash operator](../../../../../determinant-normalized-slash-operator.md) and let $\mathcal M_n$ be all integral [matrices](../../../../../matrix.md) of positive [determinant](../../../../../determinant.md) $n$. Their left $SL_2(\mathbb Z)$ cosets have the unique [determinant-n matrix representatives for Hecke operators](../../../../../determinant-n-matrix-representatives-for-hecke-operators.md)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d>0,\ ad=n,\ 0\leq b<d.
$$

Integer row operations reduce the first column to $(a,0)^T$, and a row shear then reduces $b$ modulo $d$. Define

$$
\boxed{T_nf=n^{k/2-1}\sum_{\alpha\in SL_2(\mathbb Z)\backslash\mathcal M_n}f|_k\alpha
=n^{k-1}\sum_{ad=n}d^{-k}\sum_{b=0}^{d-1}f\left(\frac{az+b}{d}\right).}
$$

Changing representatives does not affect the sum, while right multiplication by the [modular group](../../../../../modular-group.md) permutes the cosets. Hence $T_nf$ has the same modular transformation law. Rational positive-determinant slash transforms are holomorphic on $\mathbb H$ and preserve [modular cusp](../../../../../cusp-of-a-modular-group.md) vanishing: choose an integral [matrix](../../../../../matrix.md) carrying infinity to their rational image [modular cusp](../../../../../cusp-of-a-modular-group.md), after which the remaining [matrix](../../../../../matrix.md) is upper triangular. Its positive dilation sends the original decaying [modular cusp](../../../../../cusp-of-a-modular-group.md) expansion to another decaying expansion. Thus these are well-defined [Hecke operators](../../../../../hecke-operator.md) on $S_k$.

For the [Fourier expansion](../../../../../fourier-series-split.md), insert $f(z)=\sum_{m\geq1}a(m)e^{2\pi imz}$. The sum over $b$ vanishes unless $d\mid m$, in which case it is $d$. Writing $m=d\ell$, the resulting exponential is $q^{a\ell}$, and its factor is $n^{k-1}d^{1-k}=a^{k-1}$. Therefore

$$
\boxed{a(r;T_nf)=\sum_{a\mid(n,r)}a^{k-1}a(nr/a^2;f).}
$$

In particular, the first [coefficient](../../../../../coefficient.md) of $T_nf$ is $a(n;f)$.

Assume $f\ne0$ is a simultaneous [Hecke eigenform](../../../../../hecke-eigenform.md). The first-coefficient identity gives $a(n)=\lambda(n)a(1)$. If $a(1)=0$, all [coefficients](../../../../../coefficient.md) vanish, contradicting $f\ne0$. After dividing by $a(1)$, we may therefore suppose $a(1)=1$, and then $\lambda(n)=a(n)$.

We derive the relations needed for the [Euler product](../../../../../euler-product.md). For coprime $m,n$, applying the [coefficient](../../../../../coefficient.md) formula twice splits the divisors into their disjoint prime supports and yields $T_mT_n=T_{mn}$. For one prime define formal Fourier operators $U_p(\sum a(r)q^r)=\sum a(pr)q^r$ and $V_pf(z)=f(pz)$. The [coefficient](../../../../../coefficient.md) formula gives

$$
T_{p^r}=\sum_{j=0}^r p^{j(k-1)}V_p^jU_p^{r-j},\qquad U_pV_p=I.
$$

Multiplying this finite sum by $T_p=U_p+p^{k-1}V_p$ shows that

$$
T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}\qquad(r\geq1).
$$

These auxiliary operators need not separately preserve level one; the identities concern their action on [Fourier series](../../../../../fourier-series-split.md). Applied to the eigenform, they give

$$
a(mn)=a(m)a(n)\quad((m,n)=1),\qquad
a(p^{r+1})=a(p)a(p^r)-p^{k-1}a(p^{r-1}).
$$

The prime-power generating function consequently satisfies

$$
\sum_{r\geq0}a(p^r)X^r=\frac1{1-a(p)X+p^{k-1}X^2}.
$$

Multiplicativity and unique [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) now prove the [Euler product of a Hecke eigenform](../../../../../euler-product-of-a-hecke-eigenform.md):

$$
\boxed{L(f,s)=\prod_p\left(1-a(p)p^{-s}+p^{k-1-2s}\right)^{-1}.}
$$

For the original unnormalized form, the right side is multiplied by $a(1)$ and $a(p)$ in the factors is replaced by $\lambda(p)=a(p)/a(1)$. The zero form has $L=0$ and is excluded from the nonzero-eigenform product assertion.

These manipulations initially hold in an absolutely convergent right half-plane. For example, $y^{k/2}|f(z)|$ is bounded by modular invariance and [modular cusp](../../../../../cusp-of-a-modular-group.md) decay. The [coefficient](../../../../../coefficient.md) integral at $y=1/n$ gives $|a(n)|\leq Cn^{k/2}$, so $\operatorname{Re}s>k/2+1$ is sufficient. No analytic continuation is needed to justify the initial product.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
