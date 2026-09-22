<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u=(u_n)\in U_\infty$. The [Coleman interpolation theorem for cyclotomic local units](../../../../../../coleman-interpolation-theorem-for-cyclotomic-local-units.md) gives a unique [unit](../../../../../../unit-in-a-ring.md) series $f_u\in\mathbb Z_p[[T]]^\times$ with

$$
f_u(\zeta_n-1)=u_n,\qquad Nf_u=f_u.
$$

Since the entries are [principal units](../../../../../../principal-unit.md), $f_u(0)\equiv1\pmod p$. The existence statement can be seen from the norm operator as follows. Choose integral [unit](../../../../../../unit-in-a-ring.md) polynomials $F_j$ interpolating $u_j$, possible because $\mathcal O_{K_j}=\mathbb Z_p[\zeta_j-1]$. The congruence $NF\equiv F\pmod p$ and [Coleman norm contraction](../../../../../../coleman-norm-contraction.md) imply that $N^jF_{2j}$ differs from $N^{2j-m}F_{2j}$ by a factor in $1+p^{j+1}R$ for each fixed $m\leq j$. The second series evaluates at $\zeta_m-1$ to $u_m$ by repeated finite-level norms. Compactness in the $(p,T)$-adic topology gives a subsequential limit interpolating all the entries. A nonzero difference between two interpolating integral series would have infinitely many zeros in the open [unit](../../../../../../unit-in-a-ring.md) disk, contradicting the [Weierstrass preparation theorem](../../../../../../weierstrass-preparation-theorem.md). Applying the norm identity at all levels then proves norm fixation.

Set $D=(1+T)d/dT$. For $k\geq1$, define the [cyclotomic higher logarithmic derivative](../../../../../../cyclotomic-higher-logarithmic-derivative.md) by

$$
\boxed{\delta_k(u)=\left.D^{k-1}\left(\frac{Df_u}{f_u}\right)\right|_{T=0}.}
$$

The quotient $Df_u/f_u$ belongs to $\mathbb Z_p[[T]]$, and $D$ preserves that [ring](../../../../../../ring.md), so this indeed takes values in $\mathbb Z_p$. Equivalently it is $D^k\log f_u$ at zero, where the formal logarithm may be normalized by replacing $f_u$ by $f_u/f_u(0)$. There is no factorial division in this definition. Uniqueness of the [Coleman power series](../../../../../../coleman-power-series.md) gives $f_{uv}=f_uf_v$, so $\delta_k(uv)=\delta_k(u)+\delta_k(v)$.

Let $\chi_{\mathrm{cyc}}:\operatorname{Gal}(K_\infty/\mathbb Q_p)\to\mathbb Z_p^\times$ be the [cyclotomic character](../../../../../../cyclotomic-character.md), with $\sigma(\zeta_n)=\zeta_n^{\chi_{\mathrm{cyc}}(\sigma)}$. If $b=\chi_{\mathrm{cyc}}(\sigma)$, interpolation and uniqueness give

$$
f_{\sigma u}(T)=f_u((1+T)^b-1).
$$

The binomial series is integral for $b\in\mathbb Z_p$, and for any formal series $g$ the chain rule gives

$$
D\bigl(g((1+T)^b-1)\bigr)=b(Dg)((1+T)^b-1).
$$

Iteration, followed by evaluation at zero, therefore proves

$$
\boxed{\delta_k(\sigma u)=\chi_{\mathrm{cyc}}(\sigma)^k\delta_k(u).}
$$

Thus these additive [Coates–Wiles homomorphisms](../../../../../../coates-wiles-homomorphism.md) have cyclotomic weight $k$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
