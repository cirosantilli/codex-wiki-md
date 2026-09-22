<h1 id="newton-s-identities">Newton's identities</h1>

↑ **Parent:** [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton's_identities)

Newton's identities let two different summaries of the same [polynomial roots](root-of-a-polynomial.md) talk to each other. [Elementary symmetric polynomials](elementary-symmetric-polynomial.md) record products of distinct root positions; [power sums](power-sum-symmetric-polynomial.md) record sums of individual powers, $p_r=\sum_{i=1}^n x_i^r$. Either can be easier to obtain in a particular problem. The identities turn one into the other, often avoiding any need to find the individual [polynomial roots](root-of-a-polynomial.md).

Write $e_0=1$ and $e_m=0$ for $m>n$. For every positive [integer](integer.md) $m$, the identity is

$$
\boxed{m e_m=\sum_{r=1}^m(-1)^{r-1}e_{m-r}p_r}.
$$

It is a [polynomial identity](polynomial-identity.md) over the [integers](integer.md), so it remains true on substitution in any [commutative ring](commutative-ring.md). To solve it for $e_m$ by division, however, $m$ must have a [multiplicative inverse](multiplicative-inverse.md). Over a [field](field.md) of [characteristic zero](characteristic-zero.md), the first $n$ [power sums](power-sum-symmetric-polynomial.md) recover every [elementary symmetric polynomial](elementary-symmetric-polynomial.md). The same recovery works when the positive [characteristic of a field](characteristic-of-a-field.md) is greater than $n$; small characteristic needs care.[§4, p. 3, equations (30)–(37)](rational-univariate-representation-lecture-12-by-jan-verschelde.md)

The first three relations are $e_1=p_1$, $2e_2=e_1p_1-p_2$, and $3e_3=e_2p_1-e_1p_2+p_3$. When division by two and three is permitted, this becomes

$$
e_1=p_1,
\qquad
e_2=\frac{p_1^2-p_2}{2},
\qquad
e_3=\frac{p_1^3-3p_1p_2+2p_3}{6}.
$$

For the three roots $1,2,3$, their power sums are $p_1=6$, $p_2=14$, and $p_3=36$. The formulas give $e_2=(36-14)/2=11$ and $e_3=(216-252+72)/6=6$, recovering **the polynomial $z^3-6z^2+11z-6$** from aggregate data.

<a id="image-three-power-sums-reconstruct-a-cubic-without-assigning-names-to-its-roots"></a>
![](newton-identities-power-sum-reconstruction.png)

**[Figure 4](#image-three-power-sums-reconstruct-a-cubic-without-assigning-names-to-its-roots). Three power sums reconstruct a cubic without assigning names to its roots**. Left: exact contributions of the stipulated roots $1,2,3$ to the first three [power sums](power-sum-symmetric-polynomial.md). Middle: [Newton's identities](newton-s-identities.md) recover $e_1=6$, $e_2=11$, $e_3=6$. Right: the resulting [monic polynomial](monic-polynomial.md) has its three [roots of a polynomial](root-of-a-polynomial.md) at the original values. These are algebraic examples, not inferred experimental data.

The beauty is that the summaries do not depend on the order of the [polynomial roots](root-of-a-polynomial.md). In [symmetric polynomials](symmetric-polynomial.md), one can work with quantities that survive every relabeling; in [linear algebra](linear-algebra-split.md), [traces](matrix-trace.md) of [matrix powers](matrix-power.md) give the same kind of aggregate information about [eigenvalues](eigenvalue.md). The identities convert those summaries into [coefficients](coefficient.md) of a [characteristic polynomial](characteristic-polynomial.md).

A short derivation packages the identities into a [formal power series](formal-power-series.md). Let $E(t)=\prod_i(1+x_it)=\sum_{m\geq0}e_mt^m$. Since its constant coefficient is one, it has an inverse as a [formal power series](formal-power-series.md), and its [formal derivative](formal-derivative.md) satisfies

$$
\frac{E'(t)}{E(t)}=\sum_i\frac{x_i}{1+x_it}=\sum_{r\geq1}(-1)^{r-1}p_rt^{r-1}.
$$

Multiply by $E(t)$ and compare the coefficient of $t^{m-1}$. This gives [Newton's identities](newton-s-identities.md) without a convergence assumption or division by $m$. The division issue arises only when using them to recover $e_m$. The logarithmic-derivative approach is also developed in [Newton's Identities (January 2019 notes) by Milan Mossé](newton-s-identities-january-2019-notes-by-milan-mosse.md) (§4, pp. 6–8).

The alternate name [Newton-Girard identities](newton-s-identities.md) recalls [Albert Girard](albert-girard.md)'s earlier work. A modern historical account credits formulas through sixth powers to [Albert Girard](albert-girard.md) in 1629 and discusses their later appearance in [Isaac Newton](isaac-newton.md)'s Arithmetica universalis.[Newton's Identities (January 2019 notes) by Milan Mossé](newton-s-identities-january-2019-notes-by-milan-mosse.md) This citation refers to that account; the original historical editions have not been inspected here.

**Table of contents**

- [Root power-sum recurrence](root-power-sum-recurrence.md)
- [Characteristic polynomial from traces of powers](characteristic-polynomial-from-traces-of-powers.md)
- [Root sensitivity in power-sum reconstruction](root-sensitivity-in-power-sum-reconstruction.md)
- [Newton identities in positive characteristic](newton-identities-in-positive-characteristic.md)

## ↑ Ancestors (6)

1. [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Characteristic polynomial from traces of powers](characteristic-polynomial-from-traces-of-powers.md)
- [Newton's identities](newton-s-identities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13/3/solution.md)
- [Repeated-point Abel differential formula](repeated-point-abel-differential-formula.md)
- [Root power-sum recurrence](root-power-sum-recurrence.md)
- [Root sensitivity in power-sum reconstruction](root-sensitivity-in-power-sum-reconstruction.md)
