<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We first prove the simple-root [Hensel lemma](../../../../../hensel-s-lemma.md) directly. Put $x_1=x$. Suppose $x_n\equiv x\pmod\pi$ and $f(x_n)\equiv0\pmod{\pi^n}$. The derivative remains a unit since its reduction agrees with $f'(x)$. Choose $t_n\in\mathcal O_K$ whose residue solves

$$
\frac{f(x_n)}{\pi^n}+t_nf'(x_n)\equiv0\pmod\pi,
$$

and set $x_{n+1}=x_n+\pi^nt_n$. Polynomial expansion gives $f(x_{n+1})=f(x_n)+\pi^nt_nf'(x_n)+\pi^{2n}B$ with $B\in\mathcal O_K$. Since $2n\ge n+1$, the new value vanishes modulo $\pi^{n+1}$. The sequence is [Cauchy](../../../../../cauchy-sequence.md) because $v(x_{n+1}-x_n)\ge n$, and [completeness](../../../../../completeness.md) supplies $y\in\mathcal O_K$ with $y\equiv x\pmod\pi$. Continuity gives $f(y)=0$.

For uniqueness, if $y,z$ are two roots in that residue class, then

$$
0=f(y)-f(z)=(y-z)\bigl(f'(z)+(y-z)B_1\bigr),\qquad B_1\in\mathcal O_K.
$$

The factor in parentheses is a unit, since $f'(z)$ is a unit and $y-z\in\pi\mathcal O_K$. Thus $y=z$. This proves **existence and uniqueness of the specified lifted root**.

Now suppose the [residue field](../../../../../residue-field.md) has $q=p^r$ elements and put $e=v(p)$. Every element of $k_K^\times$ is a simple root of $T^{q-1}-1$. The [Hensel lemma](../../../../../hensel-s-lemma.md) therefore lifts its $q-1$ roots uniquely to a subgroup of the [roots of unity](../../../../../root-of-unity.md) in $K$. These are the [Teichmuller representatives](../../../../../teichmuller-representative.md) and give all the prime-to-$p$ torsion. To verify the latter assertion, if a [root of unity](../../../../../root-of-unity.md) $u\equiv1$ has order $m$ prime to $p$, write $u=1+t$. In $u^m-1=mt+\binom m2t^2+\cdots$, the first term has [valuation](../../../../../valuation.md) $v(t)$ and all later terms have greater [valuation](../../../../../valuation.md), so the sum cannot vanish unless $t=0$. Reduction is therefore injective on prime-to-$p$ torsion, whose order divides $q-1$.

Any [root of unity](../../../../../root-of-unity.md) has a unique decomposition into a $p$-power-order factor and a prime-to-$p$ factor, by splitting its finite order using coprime powers. For a primitive $p^a$th root $\zeta$, $a\ge1$, reduction in characteristic $p$ gives $\bar\zeta=1$. The cyclotomic identity

$$
p=\Phi_{p^a}(1)=\prod_{\substack{1\le j\le p^a\\p\nmid j}}(1-\zeta^j)
$$

shows that all factors have the same [valuation](../../../../../valuation.md): $(\zeta^j-1)/(\zeta-1)=1+\zeta+\cdots+\zeta^{j-1}$ reduces to $j\ne0$. Consequently the [valuation of a primitive p-power root of unity](../../../../../valuation-of-a-primitive-p-power-root-of-unity.md) is

$$
\boxed{v(\zeta-1)=\frac{e}{p^{a-1}(p-1)}.}
$$

The left side is a positive integer. Hence $p^{a-1}(p-1)\le e$, so the possible $p$-power orders are bounded. Combining this bound with the prime-to-$p$ result bounds all root orders by one integer, proving finiteness. A finite multiplicative subgroup of a field is cyclic, and it contains exactly the full prime-to-$p$ subgroup of order $q-1$. Thus

$$
\boxed{|\mu(K)|=p^s(q-1)\quad\text{for some }s\ge0.}
$$

If $e<p-1$, even a primitive $p$th root would violate the [valuation](../../../../../valuation.md) formula, so **$s=0$**.

At the boundary $e=p-1$, assume first that $p$ is odd. Take $K_+=\mathbb Q_p(\zeta_p)$. The polynomial $\Phi_p(1+T)=p+\binom p2T+\cdots+T^{p-1}$ is Eisenstein, so $K_+/\mathbb Q_p$ is totally ramified of degree $p-1$ and $v_{K_+}(p)=p-1$. It contains a primitive $p$th root, while the [valuation](../../../../../valuation.md) formula excludes primitive $p^2$th roots. Thus $s=1$.

For the other example, take $K_0=\mathbb Q_p(\pi)$ with $\pi^{p-1}=p$. The polynomial $T^{p-1}-p$ is Eisenstein, giving the same ramification index and [residue field](../../../../../residue-field.md) $\mathbb F_p$. If a primitive $p$th root belonged to $K_0$, the [valuation](../../../../../valuation.md) formula would give $\zeta_p-1=u\pi$ with $u$ a unit. Substitute this into $\Phi_p(1+(\zeta_p-1))=0$ and divide by $p$. All intermediate terms reduce to zero, leaving $1+\bar u^{p-1}=0$ in $\mathbb F_p$. But $\bar u^{p-1}=1$, contradicting $2\ne0$. Thus $s=0$ in $K_0$. This proves both cases of [roots of unity at the tame ramification boundary](../../../../../roots-of-unity-at-the-tame-ramification-boundary.md) for odd primes.

**The printed boundary claim needs the qualification $p>2$.** When $p=2$, every characteristic-zero field already contains the root $-1$ of order two, so $s=0$ is impossible. If $v(2)=1$, the [valuation](../../../../../valuation.md) formula excludes order four and higher, forcing $s=1$. For example $K=\mathbb Q_2$ has exactly this behavior. This is a genuine exception to the final request as printed, rather than an omitted construction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
