<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We use left multiplication by $\Gamma=SL_2(\mathbb Z)$. For an integral matrix $A$ of determinant $n>0$, the [Bezout identity](../../../../../bezout-identity.md) gives a determinant-one row operation sending its first column to $(a,0)^t$, where $a$ is the positive gcd of that column. The resulting matrix is $\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $d=n/a>0$. Adding a multiple of the second row to the first makes $0\leq b<d$.

These representatives are unique. Left multiplication by a [unimodular matrix](../../../../../unimodular-matrix.md) preserves the gcd of the first column, so two representatives in one orbit have the same $a$ and hence $d$. A matrix taking $(a,0)^t$ to itself has the form $\begin{pmatrix}1&t\\0&1\end{pmatrix}$, so it changes $b$ by $td$; the prescribed range makes $b$ unique. Thus the [determinant-n matrix representatives for Hecke operators](../../../../../determinant-n-matrix-representatives-for-hecke-operators.md) are exactly $\Pi_n$. In the printed set, $0\leq b<d$ already forces $d>0$, and $ad=n>0$ forces $a>0$.

For positive determinant extend the [slash operator for modular forms](../../../../../slash-operator-for-modular-forms.md) by

$$
(f|_k A)(z)=\det(A)^{k/2}(cz+d)^{-k}f(Az).
$$

The determinant factor makes this a right action: $(f|_k A)|_k B=f|_k(AB)$. Right multiplication by $\delta\in\Gamma$ permutes the left cosets represented by $\Pi_n$, since it preserves the set of determinant-$n$ integral matrices. Hence $T_nf$ satisfies the modular transformation law. Its summands are [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the upper half-plane. For an upper-triangular representative,

$$
T_nf=n^{k-1}\sum_{ad=n\atop a,d>0}d^{-k}
\sum_{b=0}^{d-1}f\left(\frac{az+b}{d}\right).
$$

Substitute the [Fourier expansion of a modular form](../../../../../fourier-expansion-of-a-modular-form.md). The sum over $b$ is zero unless the original index is divisible by $d$, in which case it equals $d$. Writing that index as $dr$ gives

$$
T_nf=\sum_{ad=n\atop a,d>0}a^{k-1}\sum_{r\geq0}a_{dr}(f)q^{ar}.
$$

Only nonnegative powers occur, so $T_nf$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) at infinity, and all level-one cusps are equivalent to infinity. We have proved $T_nf\in M_k(\Gamma)$ and the [Fourier coefficients of a composite-index Hecke operator](../../../../../fourier-coefficients-of-a-composite-index-hecke-operator.md) formula

$$
\boxed{a_r(T_nf)=\sum_{a\mid\gcd(n,r)}a^{k-1}a_{nr/a^2}(f)
\quad(r\geq0),\qquad a_1(T_nf)=a_n(f).}
$$

Here $\gcd(n,0)=n$, giving $a_0(T_nf)=\sum_{a\mid n}a^{k-1}a_0(f)$. In particular [cusp forms](../../../../../cusp-form.md) stay [cusp forms](../../../../../cusp-form.md). For nonzero level-one [cusp forms](../../../../../cusp-form.md) the weight is an even integer at least twelve, so the powers $a^{k-1}$ are integers; the zero cusp space causes no exception. Thus every $T_n$ preserves integral [Fourier coefficients](../../../../../fourier-coefficient.md), and closure under addition, multiplication and integer scalars proves

$$
\boxed{\mathbb T\,S_k(\Gamma,\mathbb Z)\subseteq S_k(\Gamma,\mathbb Z).}
$$

This is the [integral Hecke algebra of level-one cusp forms](../../../../../integral-hecke-algebra-of-level-one-cusp-forms.md).

We will also need commutativity. The coefficient formula directly gives

$$
T_uT_v=T_{uv}\quad(\gcd(u,v)=1),\qquad
T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}\quad(r\geq1).
$$

For the first identity, the divisors of $u$ and $v$ in the iterated coefficient sum combine uniquely into a divisor of $uv$. For the second, write a coefficient index as $p^t r_0$ with $p\nmid r_0$; the formula is

$$
a_{p^t r_0}(T_{p^r}f)=\sum_{j=0}^{\min(r,t)}p^{j(k-1)}a_{p^{r+t-2j}r_0}(f).
$$

Applying $T_p$ splits this into the two sums with shifts $t+1$ and $t-1$; their overlapping terms give exactly the stated recurrence. Since $T_1$ is the identity, induction expresses each $T_{p^r}$ as a polynomial in $T_p$, and coprime multiplicativity expresses every $T_n$ as a product of these polynomials. Distinct prime operators commute by the coprime identity. Hence all [Hecke operators](../../../../../hecke-operator.md) commute, and so do all elements of $\mathbb T$.

Let $\Lambda=S_k(\Gamma,\mathbb Z)$ and $m=\dim S_k(\Gamma)$. In the permitted [basis](../../../../../basis.md) $F_j=\Delta^jE_4^{a_j}E_6^{b_j}$, the [modular discriminant](../../../../../modular-discriminant.md) begins $q+O(q^2)$ and the normalized [Eisenstein series](../../../../../eisenstein-series.md) begin $1+O(q)$, so

$$
F_j=q^j+O(q^{j+1})\quad(1\leq j\leq m).
$$

The matrix of $a_1,\ldots,a_m$ on this integral [basis](../../../../../basis.md) is unitriangular and has determinant one. Integer elimination therefore gives an integral [basis](../../../../../basis.md) $f_1,\ldots,f_m$ with $a_i(f_j)=\delta_{ij}$ for $1\leq i,j\leq m$. Thus $a_1,\ldots,a_m$ are a $\mathbb Z$-basis of the [dual module](../../../../../dual-module.md) $\operatorname{Hom}_{\mathbb Z}(\Lambda,\mathbb Z)$.

The map $\alpha$ is well-defined by lattice preservation and is $\mathbb Z$-linear. Because $\alpha(T_j)=a_j$, it is surjective. For injectivity suppose $\alpha(T)=0$. For every $f\in\Lambda$ and every $n\geq1$, commutativity gives

$$
a_n(Tf)=a_1(T_nTf)=a_1(TT_nf)=\alpha(T)(T_nf)=0.
$$

The constant term is also zero because $Tf$ is a [cusp form](../../../../../cusp-form.md). The [identity theorem](../../../../../identity-theorem.md) applied to its [Fourier expansion of a modular form](../../../../../fourier-expansion-of-a-modular-form.md) gives $Tf=0$. The integral [basis](../../../../../basis.md) spans the complex cusp space, so $T=0$ as an endomorphism. This proves the [perfect integral Hecke pairing](../../../../../perfect-integral-hecke-pairing.md) and

$$
\boxed{\mathbb T\cong\operatorname{Hom}_{\mathbb Z}(\Lambda,\mathbb Z),
\qquad\mathbb T=\bigoplus_{j=1}^m\mathbb ZT_j.}
$$

If $m=0$, both modules are zero and the asserted [basis](../../../../../basis.md) is empty.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
