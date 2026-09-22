<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $M_f$ be the [matrix](../../../../../matrix.md) of multiplication by $f$ in the [basis](../../../../../basis.md) from Question 1. Define the [Coleman norm operator](../../../../../coleman-norm-operator.md) by the [norm for a finite free ring extension](../../../../../norm-for-a-finite-free-ring-extension.md):

$$
\boxed{\phi(Nf)=\det(M_f).}
$$

The entries lie in $\phi(R)$, and $\phi:R\to\phi(R)$ is an [isomorphism](../../../../../isomorphism.md), so this determines $Nf$ uniquely. If $f$ is a [unit](../../../../../unit-in-a-ring.md), $M_f$ is invertible and its [determinant](../../../../../determinant.md) is a [unit](../../../../../unit-in-a-ring.md). Also $M_{fg}=M_fM_g$, giving $N(fg)=Nf\,Ng$. Splitting the conjugates, or diagonalizing multiplication after adjoining the [roots of unity](../../../../../root-of-unity.md) and inverting $p$, gives the equivalent formula

$$
\phi(Nf)(T)=\prod_{\zeta\in\mu_p}f(\zeta(1+T)-1).
$$

In particular, this definition has the required target $R^\times$, rather than merely a [ring](../../../../../ring.md) with extra [roots of unity](../../../../../root-of-unity.md) in its coefficients.

For the requested [ring congruence](../../../../../congruence-modulo-an-ideal.md), observe that the reduction of $\phi$ is the injective map $\overline g(T)\mapsto\overline g(T^p)$. If $\phi(g)\in p^kR$, its reduction first gives $g=pg_1$. Then $\phi(g_1)\in p^{k-1}R$; repeat to obtain $g\in p^kR$. Applying this to $g=f-1$ proves

$$
\boxed{\phi(f)\equiv1\pmod{p^kR}\ \Longrightarrow\ f\equiv1\pmod{p^kR}.}
$$

This [congruence reflection for Frobenius substitution](../../../../../congruence-reflection-for-frobenius-substitution.md) is valid for all $f\in R$, without assuming $f$ is a [unit](../../../../../unit-in-a-ring.md).

A further property needed for the fixed points is [Coleman norm contraction](../../../../../coleman-norm-contraction.md). If $g=1+p^kh$ with $k\geq1$, expand the [determinant](../../../../../determinant.md):

$$
\phi(Ng)=\det(I+p^kM_h)=1+p^k\operatorname{Tr}(M_h)+\sum_{j=2}^{p}p^{kj}e_j(M_h).
$$

Here $e_j(M_h)\in\phi(R)$ is the coefficient of degree $j$ in $\det(I+tM_h)$. The [trace](../../../../../matrix-trace.md) formula from Question 1 makes the linear term divisible by $p^{k+1}$; every later term is divisible by $p^{2k}$ and $2k\geq k+1$. Reflecting the resulting [ring congruence](../../../../../congruence-modulo-an-ideal.md) through $\phi$ gives

$$
N(1+p^kR)\subseteq1+p^{k+1}R.
$$

If $Nf=f$ and $f\in1+pR$, iteration gives $f\in1+p^kR$ for every $k$. Since $\bigcap_k p^kR=0$, **$f=1$**.

To identify all fixed points, we also need $Nf\equiv f\pmod{pR}$ for every [unit](../../../../../unit-in-a-ring.md) $f$. In characteristic $p$, the extension $\mathbb F_p[[T]]/\mathbb F_p[[T^p]]$ has degree $p$ and its [norm for a finite free ring extension](../../../../../norm-for-a-finite-free-ring-extension.md) is $\overline f\mapsto\overline f^{\,p}$. Indeed, after passing to [fraction fields](../../../../../field-of-fractions.md) it is a [purely inseparable field extension](../../../../../purely-inseparable-extension.md) of degree $p$, so multiplication has only the [eigenvalue](../../../../../eigenvalue.md) $\overline f$, with multiplicity $p$, after splitting. Its [determinant](../../../../../determinant.md) is $\overline f^{\,p}$. Therefore

$$
\overline{\phi(Nf)}=\overline f^{\,p}=\overline{\phi(f)},
$$

and [congruence reflection for Frobenius substitution](../../../../../congruence-reflection-for-frobenius-substitution.md) gives $Nf\equiv f\pmod{pR}$.

Now choose any lift $f_0\in R^\times$ of a given $a\in A^\times$ and put $f_n=N^nf_0$. Multiplicativity gives

$$
\frac{f_{n+1}}{f_n}=N^n\left(\frac{Nf_0}{f_0}\right)\in1+p^{n+1}R.
$$

Thus $(f_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) for the finer of the [topologies on integral formal power series](../../../../../topologies-on-integral-formal-power-series.md) and converges to a [unit](../../../../../unit-in-a-ring.md) $w(a)$ reducing to $a$. The [Coleman norm operator](../../../../../coleman-norm-operator.md) is continuous: multiplication matrices and their [determinants](../../../../../determinant.md) are continuous, and the finite-free coordinate decomposition and its inverse preserve the $p$-adic filtration defining the finer of the [topologies on integral formal power series](../../../../../topologies-on-integral-formal-power-series.md). Hence $Nw(a)=w(a)$. If two fixed [units](../../../../../unit-in-a-ring.md) reduce to $a$, their quotient is fixed and belongs to $1+pR$, so it is $1$ by the preceding argument. This proves uniqueness, independence of the initial lift, and multiplicativity of the [Coleman norm-fixed lift](../../../../../coleman-norm-fixed-lift.md). In particular,

$$
\boxed{W\xrightarrow[\text{reduction}]{\ \sim\ }A^\times,\qquad a\longmapsto w(a)=\lim_{n\to\infty}N^nf_0\text{ in the inverse direction}.}
$$

Every [unit](../../../../../unit-in-a-ring.md) $f\in R$ consequently has a unique factorization $f=w(\overline f)v$ with $v\in1+pR$, giving the [canonical Coleman decomposition of power-series units](../../../../../canonical-coleman-decomposition-of-power-series-units.md):

$$
\boxed{R^\times\simeq W\times(1+pR),\qquad f\longmapsto\left(w(\overline f),\frac{f}{w(\overline f)}\right).}
$$

**The final assertion as printed is false.** The original PDF identifies a [ring](../../../../../ring.md) with a product of [unit groups](../../../../../unit-group.md). With multiplication, $A$ has a zero and is not a [group](../../../../../group-split.md). With addition, it has exponent $p$, whereas $W\times A^\times$ has a nonidentity element of order $2$: $-1\in W$ because $p$ is odd and $N(-1)=(-1)^p=-1$. Thus neither interpretation makes the printed assertion true. The two boxed isomorphisms above are the valid natural conclusions; they do not require guessing which symbols the author intended to replace.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
