<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $p\nmid2k$, the displayed integral equation has nonzero [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) modulo $p$, so it has [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md). Let $\chi$ be the [Legendre symbol](../../../../../../legendre-symbol.md), with $\chi(0)=0$. Counting the two, one, or zero possible ordinates over each $x$ gives

$$
\#\widetilde E(\mathbb F_p)=p+1+\sum_{x\in\mathbb F_p}\chi(x^3+kx).
$$

If $p\equiv3\pmod4$, then $\chi(-1)=-1$ and the terms for $x$ and $-x$ cancel. The term at zero vanishes. Thus the count is $p+1$.

For the converse, suppose $p\equiv1\pmod4$, and put $h=(p-1)/2$. The [Euler criterion](../../../../../../euler-criterion.md) and the sum of powers over a [finite field](../../../../../../finite-field.md) show that the [Trace of Frobenius](../../../../../../trace-of-frobenius.md) satisfies

$$
a_p=-\sum_x\chi(x^3+kx)\equiv[x^{p-1}](x^3+kx)^h\pmod p.
$$

Indeed, among the positive exponents in this polynomial, of degree $3(p-1)/2<2(p-1)$, only $p-1$ has a nonzero sum over $\mathbb F_p$, and that sum is $-1$. Since $(x^3+kx)^h=x^h(x^2+k)^h$, the [coefficient formula for trace of Frobenius modulo p](../../../../../../coefficient-formula-for-trace-of-frobenius-modulo-p.md) yields

$$
a_p\equiv\binom{h}{h/2}k^{h/2}\not\equiv0\pmod p.
$$

Neither $k$ nor the [binomial coefficient](../../../../../../binomial-coefficient.md) vanishes modulo $p$. Hence $a_p\ne0$, proving the [point-count criterion for y squared equals x cubed plus k x](../../../../../../point-count-criterion-for-y-squared-equals-x-cubed-plus-k-x.md):

$$
\boxed{\#\widetilde E(\mathbb F_p)=p+1\iff p\equiv3\pmod4.}
$$

We use the following [formal logarithm](../../../../../../formal-logarithm.md) fact, also useful for the next part. For a [formal group law](../../../../../../formal-group-law.md) over $\mathbb Z_p$, its logarithm has coefficients $c_j/j$ with $c_j\in\mathbb Z_p$, obtained by integrating its integral invariant differential. If $p$ is odd and $t\in p\mathbb Z_p\setminus\{0\}$, every term of degree $j\geq2$ has [valuation](../../../../../../valuation.md) strictly greater than $v_p(t)$, since $jv_p(t)-v_p(j)>v_p(t)$. Thus the logarithm converges and is nonzero at $t$. Its homomorphism into the additive characteristic-zero group proves [torsion-freeness of the formal group over Qp for odd p](../../../../../../torsion-freeness-of-the-formal-group-over-qp-for-odd-p.md). Consequently reduction injects the entire rational [torsion subgroup](../../../../../../torsion-subgroup.md) at any odd [prime](../../../../../../prime-number.md) of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), including its $p$-primary torsion. In particular the [torsion subgroup](../../../../../../torsion-subgroup.md) is finite, and its order divides $p+1$ at every good $p\equiv3\pmod4$.

By the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md), choose a good [prime](../../../../../../prime-number.md) $p\equiv3\pmod8$. Then $v_2(p+1)=2$, bounding the two-primary part by four. For any odd [prime](../../../../../../prime-number.md) $\ell$ dividing the torsion order, the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) and the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) give a good [prime](../../../../../../prime-number.md) $p$ with $p\equiv3\pmod4$ and $p\equiv1\pmod\ell$, avoiding the finitely many [primes](../../../../../../prime-number.md) dividing $2k$. But then $\ell\nmid p+1$, a contradiction. Therefore

$$
\boxed{\#E(\mathbb Q)_{\rm tors}\mid4.}
$$

The order four does occur. For $k=4$, the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives $2(2,4)=(0,0)$, so $(2,4)$ has order four. More precisely, the only nonzero rational [2-torsion](../../../../../../2-torsion.md) point when $k>0$ is $(0,0)$, so order four means a cyclic group with a rational half of this point. The duplication formula is

$$
x(2P)=\frac{(x(P)^2-k)^2}{4x(P)(x(P)^2+k)}.
$$

Such a half must have $x(P)^2=k$. Writing $k=s^2$, positivity of $y(P)^2=2kx(P)$ forces $x(P)=s>0$. Then $y(P)^2=2s^3$, so $2s$ is a rational square, equivalently $s=2t^2$ for an integer $t\geq1$. Conversely $(2t^2,4t^3)$ is a half of $(0,0)$ when $k=4t^4$. The [rational torsion on y squared equals x cubed plus positive k x](../../../../../../rational-torsion-on-y-squared-equals-x-cubed-plus-positive-k-x.md) is therefore cyclic of order four exactly for these $k$, and otherwise cyclic of order two.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
