# Paper 27

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper27.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper27.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Every nonzero [P-adic number](../../../arithmetic.md#p-adic-number) has a unique decomposition $z=p^mu$ with $m\in\mathbb Z$ and $u\in\mathbb Z_p^\times$. The [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) of reduction from the [unit group](../../../algebra.md#unit-group) onto $\mathbb F_p^\times$ is $1+p\mathbb Z_p$, the group of [principal units](../../../arithmetic.md#principal-unit). Each nonzero residue class has a unique lift $\omega$ satisfying $\omega^{p-1}=1$, by the simple-root [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) proved in question 3. Uniqueness makes these lifts multiplicative. They form the [cyclic group](../../../group.md#cyclic-group) $\mu_{p-1}$, and every unit has a unique factorization

$$
u=\omega\,v,\qquad\omega\in\mu_{p-1},\quad v\in1+p\mathbb Z_p.
$$

Thus $\mathbb Q_p^\times=p^{\mathbb Z}\times\mu_{p-1}\times(1+p\mathbb Z_p)$.

For odd $p$, the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) and [p-adic exponential function](../../../arithmetic.md#p-adic-exponential-function) give inverse group isomorphisms $1+p\mathbb Z_p\leftrightarrow p\mathbb Z_p$. To verify the convergence domain, for $t\in p\mathbb Z_p$ the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) terms have valuations $nv_p(t)-v_p(n)\to\infty$, and the exponential terms have valuations $nv_p(t)-v_p(n!)\to\infty$, since $v_p(n!)\le(n-1)/(p-1)$ and $p>2$. In both series every term after the linear one has strictly larger [valuation](../../../algebra.md#valuation) than the linear term. Consequently $\log(1+t)\in p\mathbb Z_p$ and $\exp(t)\in1+p\mathbb Z_p$. The formal identities $\log(vw)=\log v+\log w$ and $\exp(\log v)=v$, $\log(\exp t)=t$ hold on these convergent domains, as follows by multiplying the convergent series or passing to their formal identities termwise.

Choose a generator $\zeta$ of $\mu_{p-1}$. An explicit isomorphism is

$$
\boxed{\mathbb Z/(p-1)\mathbb Z\times\mathbb Z_p\times\mathbb Z\longrightarrow\mathbb Q_p^\times,\qquad(a,b,m)\longmapsto\zeta^a\exp(pb)p^m.}
$$

The inverse reads off the [valuation](../../../algebra.md#valuation), the root-of-unity unit factor, and $p^{-1}\log(v)$. Both directions are continuous with the standard product topology, so this is also a [topological group](../../../topological-group.md) isomorphism. The odd-prime condition is essential for using all of $1+p\mathbb Z_p$ as the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm)-isomorphism domain.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For a finite extension of fields [complete](../../../topological-analysis.md#completeness) for a [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value), use the unique extended [field absolute value](../../../arithmetic.md#absolute-value-algebra). The extension is [unramified](../../../arithmetic.md#unramified-extension) when its residue extension is a [separable field extension](../../../galois-theory.md#separable-extension) and

$$
[L:K]=[k_L:k_K].
$$

Equivalently, it has ramification index one, a [separable field extension](../../../galois-theory.md#separable-extension) of residue fields, and no defect. For general nondiscrete valued fields, merely saying that the ramification index is one is insufficient; the displayed degree equality is part of the unramified condition.

Put $n=[L:K]=[k_L:k_K]$. Since $\bar x$ generates the residue extension, $1,\bar x,\ldots,\bar x^{n-1}$ are [linearly independent](../../../vector-space.md#linear-independence) over $k_K$. Their lifts $1,x,\ldots,x^{n-1}$ are [linearly independent](../../../vector-space.md#linear-independence) over $K$: a nonzero relation could be divided by a coefficient of largest [field absolute value](../../../arithmetic.md#absolute-value-algebra), giving an integral relation whose reduction has at least one nonzero coefficient, contrary to residue independence. They therefore form a $K$-[basis](../../../vector-space.md#basis) of $L$.

For any $y=\sum_{j=0}^{n-1}a_jx^j$, choose $a_r$ of largest [field absolute value](../../../arithmetic.md#absolute-value-algebra). All coefficients of $y/a_r$ belong to $\mathcal O_K$, and at least one is a unit. Its reduction is a nonzero linear combination of the residue [basis](../../../vector-space.md#basis), so $y/a_r$ is a unit of $\mathcal O_L$. This proves the [residue-basis norm formula for an unramified extension](../../../arithmetic.md#residue-basis-norm-formula-for-an-unramified-extension)

$$
|y|=\max_j|a_j|.
$$

Hence $y\in\mathcal O_L$ exactly when every $a_j\in\mathcal O_K$. We conclude

$$
\boxed{\mathcal O_L=\bigoplus_{j=0}^{n-1}\mathcal O_Kx^j=\mathcal O_K[x].}
$$

The last equality also uses the fact that every polynomial in the integral element $x$ is integral. The proof requires neither a [uniformizer](../../../commutative-algebra.md#uniformizer) nor discrete [valuation](../../../algebra.md#valuation), and applies to every residue generator specified in the question.

## 2

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Mahler theorem](../../../arithmetic.md#mahler-s-theorem) states that a function $f:\mathbb Z_p\to\mathbb Q_p$ is continuous if and only if it has a unique expansion

$$
f(x)=\sum_{n\ge0}c_n\binom xn,\qquad c_n\in\mathbb Q_p,\quad c_n\longrightarrow0,
$$

and the expansion converges uniformly. Moreover $\|f\|_\infty=\sup_n|c_n|_p$; in particular $f$ takes values in $\mathbb Z_p$ exactly when all $c_n$ belong to $\mathbb Z_p$. Here $\binom{x}{0}=1$ and $\binom{x}{n}=x(x-1)\cdots(x-n+1)/n!$. These [binomial polynomials](../../../commutative-algebra.md#binomial-polynomial) are continuous and integer-valued on $\mathbb Z_p$, since they are integer-valued on the dense nonnegative integers. The coefficient condition $c_n\to0$ therefore makes the series uniformly convergent.

Evaluate at a nonnegative integer $m$. Terms with $n>m$ vanish, giving the finite triangular relation $f(m)=\sum_{n=0}^m\binom mn c_n$. [Binomial inversion](../../../combinatorics.md#binomial-inversion) gives the [Mahler coefficients](../../../arithmetic.md#mahler-coefficient)

$$
\boxed{c_n=\sum_{j=0}^n(-1)^{n-j}\binom njf(j)=(\Delta^nf)(0),\qquad\Delta f(x)=f(x+1)-f(x).}
$$

To obtain the generating function, multiply the last finite identity by $T^n/n!$ and compare coefficients. Setting $n=j+k$ yields

$$
\sum_{n\ge0}\frac{c_n}{n!}T^n=\sum_{j,k\ge0}\frac{(-1)^k f(j)}{j!k!}T^{j+k}=\boxed{e^{-T}\sum_{j\ge0}\frac{f(j)}{j!}T^j.}
$$

The [Mahler coefficient exponential generating function](../../../arithmetic.md#mahler-coefficient-exponential-generating-function) is an identity in $\mathbb Q_p[[T]]$: each coefficient is a finite sum. It does not assert convergence for every $p$-adic substitution for $T$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $c_n$ be the [Mahler coefficients](../../../arithmetic.md#mahler-coefficient) of $f$. Define its [discrete antiderivative](../../../finite-difference.md#discrete-antiderivative) by

$$
\boxed{g(x)=\sum_{n\ge0}c_n\binom{x}{n+1}.}
$$

Because $c_n\to0$ and the [binomial polynomials](../../../commutative-algebra.md#binomial-polynomial) have [field absolute value](../../../arithmetic.md#absolute-value-algebra) at most one on $\mathbb Z_p$, this series converges uniformly to a continuous $\mathbb Z_p$-valued function. Every summand vanishes at zero. [Pascal's identity](../../../combinatorics.md#pascal-s-rule) gives $\binom{x+1}{n+1}-\binom{x}{n+1}=\binom xn$, so taking differences through the uniformly convergent series proves $g(x+1)-g(x)=f(x)$. For nonnegative integers, induction from $g(0)=0$ gives precisely $g(m)=\sum_{j=0}^{m-1}f(j)$. Thus this is the required continuous extension, unique because the nonnegative integers are dense in $\mathbb Z_p$.

The [Mahler expansion](../../../arithmetic.md#mahler-s-theorem) of $g$ has coefficient zero in degree zero and coefficient $c_{m-1}$ in degree $m\ge1$. This [discrete antidifferentiation on the p-adic integers](../../../arithmetic.md#discrete-antidifferentiation-on-the-p-adic-integers) is the mechanism behind the next part.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Take an arbitrary $f\in C(\mathbb Z_p,\mathbb Q_p)$. Compactness of $\mathbb Z_p$ bounds its [field absolute value](../../../arithmetic.md#absolute-value-algebra), so some $p^mf$ takes values in $\mathbb Z_p$. Apply part (ii) to obtain a continuous $h$ with $h(x+1)-h(x)=p^mf(x)$. Then $g=p^{-m}h$ belongs to the same continuous-function space and satisfies $f=g(\cdot+1)-g$.

Translation invariance by one alone now gives $L(f)=L(g(\cdot+1))-L(g)=0$. Since $f$ was arbitrary,

$$
\boxed{L=0.}
$$

This proves [translation-invariant linear forms on p-adic continuous functions vanish](../../../arithmetic.md#translation-invariant-linear-forms-on-p-adic-continuous-functions-vanish) without assuming that the [linear form](../../../linear-algebra.md#linear-functional) itself is continuous. A proof using only density of polynomials would not suffice for an arbitrary, potentially discontinuous [linear form](../../../linear-algebra.md#linear-functional); surjectivity of the [forward difference operator](../../../finite-difference.md#forward-difference-operator) on the entire function space is what is needed.

## 3

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We first prove the simple-root [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) directly. Put $x_1=x$. Suppose $x_n\equiv x\pmod\pi$ and $f(x_n)\equiv0\pmod{\pi^n}$. The derivative remains a unit since its reduction agrees with $f'(x)$. Choose $t_n\in\mathcal O_K$ whose residue solves

$$
\frac{f(x_n)}{\pi^n}+t_nf'(x_n)\equiv0\pmod\pi,
$$

and set $x_{n+1}=x_n+\pi^nt_n$. Polynomial expansion gives $f(x_{n+1})=f(x_n)+\pi^nt_nf'(x_n)+\pi^{2n}B$ with $B\in\mathcal O_K$. Since $2n\ge n+1$, the new value vanishes modulo $\pi^{n+1}$. The sequence is [Cauchy](../../../real-analysis.md#cauchy-sequence) because $v(x_{n+1}-x_n)\ge n$, and [completeness](../../../topological-analysis.md#completeness) supplies $y\in\mathcal O_K$ with $y\equiv x\pmod\pi$. Continuity gives $f(y)=0$.

For uniqueness, if $y,z$ are two roots in that residue class, then

$$
0=f(y)-f(z)=(y-z)\bigl(f'(z)+(y-z)B_1\bigr),\qquad B_1\in\mathcal O_K.
$$

The factor in parentheses is a unit, since $f'(z)$ is a unit and $y-z\in\pi\mathcal O_K$. Thus $y=z$. This proves **existence and uniqueness of the specified lifted root**.

Now suppose the [residue field](../../../commutative-algebra.md#residue-field) has $q=p^r$ elements and put $e=v(p)$. Every element of $k_K^\times$ is a simple root of $T^{q-1}-1$. The [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) therefore lifts its $q-1$ roots uniquely to a subgroup of the [roots of unity](../../../algebra.md#root-of-unity) in $K$. These are the [Teichmuller representatives](../../../arithmetic.md#teichmuller-representative) and give all the prime-to-$p$ torsion. To verify the latter assertion, if a [root of unity](../../../algebra.md#root-of-unity) $u\equiv1$ has order $m$ prime to $p$, write $u=1+t$. In $u^m-1=mt+\binom m2t^2+\cdots$, the first term has [valuation](../../../algebra.md#valuation) $v(t)$ and all later terms have greater [valuation](../../../algebra.md#valuation), so the sum cannot vanish unless $t=0$. Reduction is therefore injective on prime-to-$p$ torsion, whose order divides $q-1$.

Any [root of unity](../../../algebra.md#root-of-unity) has a unique decomposition into a $p$-power-order factor and a prime-to-$p$ factor, by splitting its finite order using coprime powers. For a primitive $p^a$th root $\zeta$, $a\ge1$, reduction in characteristic $p$ gives $\bar\zeta=1$. The cyclotomic identity

$$
p=\Phi_{p^a}(1)=\prod_{\substack{1\le j\le p^a\\p\nmid j}}(1-\zeta^j)
$$

shows that all factors have the same [valuation](../../../algebra.md#valuation): $(\zeta^j-1)/(\zeta-1)=1+\zeta+\cdots+\zeta^{j-1}$ reduces to $j\ne0$. Consequently the [valuation of a primitive p-power root of unity](../../../arithmetic.md#valuation-of-a-primitive-p-power-root-of-unity) is

$$
\boxed{v(\zeta-1)=\frac{e}{p^{a-1}(p-1)}.}
$$

The left side is a positive integer. Hence $p^{a-1}(p-1)\le e$, so the possible $p$-power orders are bounded. Combining this bound with the prime-to-$p$ result bounds all root orders by one integer, proving finiteness. A finite multiplicative subgroup of a field is cyclic, and it contains exactly the full prime-to-$p$ subgroup of order $q-1$. Thus

$$
\boxed{|\mu(K)|=p^s(q-1)\quad\text{for some }s\ge0.}
$$

If $e<p-1$, even a primitive $p$th root would violate the [valuation](../../../algebra.md#valuation) formula, so **$s=0$**.

At the boundary $e=p-1$, assume first that $p$ is odd. Take $K_+=\mathbb Q_p(\zeta_p)$. The polynomial $\Phi_p(1+T)=p+\binom p2T+\cdots+T^{p-1}$ is Eisenstein, so $K_+/\mathbb Q_p$ is totally ramified of degree $p-1$ and $v_{K_+}(p)=p-1$. It contains a primitive $p$th root, while the [valuation](../../../algebra.md#valuation) formula excludes primitive $p^2$th roots. Thus $s=1$.

For the other example, take $K_0=\mathbb Q_p(\pi)$ with $\pi^{p-1}=p$. The polynomial $T^{p-1}-p$ is Eisenstein, giving the same ramification index and [residue field](../../../commutative-algebra.md#residue-field) $\mathbb F_p$. If a primitive $p$th root belonged to $K_0$, the [valuation](../../../algebra.md#valuation) formula would give $\zeta_p-1=u\pi$ with $u$ a unit. Substitute this into $\Phi_p(1+(\zeta_p-1))=0$ and divide by $p$. All intermediate terms reduce to zero, leaving $1+\bar u^{p-1}=0$ in $\mathbb F_p$. But $\bar u^{p-1}=1$, contradicting $2\ne0$. Thus $s=0$ in $K_0$. This proves both cases of [roots of unity at the tame ramification boundary](../../../arithmetic.md#roots-of-unity-at-the-tame-ramification-boundary) for odd primes.

**The printed boundary claim needs the qualification $p>2$.** When $p=2$, every characteristic-zero field already contains the root $-1$ of order two, so $s=0$ is impossible. If $v(2)=1$, the [valuation](../../../algebra.md#valuation) formula excludes order four and higher, forcing $s=1$. For example $K=\mathbb Q_2$ has exactly this behavior. This is a genuine exception to the final request as printed, rather than an omitted construction.

## 4

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [valuation ring](../../../commutative-algebra.md#valuation-ring) is $\mathcal O=\{x\in K:|x|\le1\}$, and $\mathfrak m=\{x\in K:|x|<1\}$ is an ideal by the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality). Its complement inside $\mathcal O$ consists exactly of elements of [field absolute value](../../../arithmetic.md#absolute-value-algebra) one, whose inverses also lie in $\mathcal O$. Every proper ideal must avoid units and hence lie in $\mathfrak m$. Therefore $\mathfrak m$ is the unique [maximal ideal](../../../commutative-algebra.md#maximal-ideal): **$\mathcal O$ is a [local ring](../../../commutative-algebra.md#local-ring)**. Also its fraction field is $K$, since every nonzero element outside the ring has its inverse inside it.

If $z\in K$ is integral over $\mathcal O$, it satisfies a monic equation $z^n+a_{n-1}z^{n-1}+\cdots+a_0=0$ with $|a_i|\le1$. Were $|z|>1$, the leading term would have strictly larger [field absolute value](../../../arithmetic.md#absolute-value-algebra) than every other term, so the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) would prevent cancellation to zero. Thus $z\in\mathcal O$, proving **the [valuation ring](../../../commutative-algebra.md#valuation-ring) is integrally closed**.

For the ideal criterion, assume the [valuation](../../../algebra.md#valuation) is nontrivial and write $v=-\log|\cdot|$. If its [value group](../../../commutative-algebra.md#value-group) is discrete, normalize it to $\mathbb Z$ and choose a [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$ of [valuation](../../../algebra.md#valuation) one. In any nonzero ideal $I$, the nonnegative integer valuations have a least value $m$. Choose $a\in I$ of that value. For every $b\in I$, $v(b/a)\ge0$, so $b\in a\mathcal O$. Hence $I=(a)=(\pi^m)$ and $\mathcal O$ is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain).

Conversely, if $\mathcal O$ is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), its nonzero [maximal ideal](../../../commutative-algebra.md#maximal-ideal) is $(\pi)$. For every element $x$ of positive [valuation](../../../algebra.md#valuation), $x\in\mathfrak m$ implies $x=\pi y$ with $y\in\mathcal O$, so $v(x)\ge v(\pi)>0$. Thus $\gamma=v(\pi)$ is the least positive value. For any value $t$, subtract $\lfloor t/\gamma\rfloor\gamma$. The remainder belongs to the [value group](../../../commutative-algebra.md#value-group) and lies in $[0,\gamma)$, so is zero. The [value group](../../../commutative-algebra.md#value-group) is therefore $\gamma\mathbb Z$, and the [valuation](../../../algebra.md#valuation) is discrete. We have proved the [principal ideal criterion for a nontrivial rank-one valuation ring](../../../commutative-algebra.md#principal-ideal-criterion-for-a-nontrivial-rank-one-valuation-ring).

The nontriviality qualification matters under the standard definition of [discrete valuation](../../../commutative-algebra.md#discrete-valuation), which requires [value group](../../../commutative-algebra.md#value-group) isomorphic to $\mathbb Z$. With the trivial [field absolute value](../../../arithmetic.md#absolute-value-algebra), $\mathcal O=K$ is still a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), but the [value group](../../../commutative-algebra.md#value-group) is zero and there is no [uniformizer](../../../commutative-algebra.md#uniformizer). Thus the literal unrestricted equivalence has a field exception. If “discrete” instead includes the trivial [value group](../../../commutative-algebra.md#value-group) as a discrete subgroup of $\mathbb R$, that exceptional case satisfies the equivalence too.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

[Krasner's lemma](../../../arithmetic.md#krasner-s-lemma) states: let $K$ be [complete](../../../topological-analysis.md#completeness) for a [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value), let $\alpha$ be a [separable algebraic element](../../../galois-theory.md#separable-algebraic-element) over $K$, and let $\beta$ be algebraic over $K$, all in a fixed [algebraic closure](../../../algebra.md#algebraic-closure) with the extended [field absolute value](../../../arithmetic.md#absolute-value-algebra). If

$$
|\beta-\alpha|<|\alpha'-\alpha|\quad\text{for every }K\text{-conjugate }\alpha'\ne\alpha,
$$

then $K(\alpha)\subseteq K(\beta)$. If $\alpha\in K$, the conclusion is automatic and there is no conjugate-distance condition to check.

To prove it, put $F=K(\beta)$ and take a finite splitting field $N/F$ for the minimal polynomial of $\alpha$ over $F$. That is a [separable polynomial](../../../galois-theory.md#separable-polynomial), so $N/F$ is Galois. The finite extension $F$ is [complete](../../../topological-analysis.md#completeness), and uniqueness of extensions of an [field absolute value](../../../arithmetic.md#absolute-value-algebra) from a [complete](../../../topological-analysis.md#completeness) non-Archimedean field makes every $\sigma\in\operatorname{Gal}(N/F)$ an isometry. It fixes $\beta$, so

$$
|\sigma(\alpha)-\alpha|\le\max\{|\sigma(\alpha)-\beta|,|\beta-\alpha|\}=|\beta-\alpha|.
$$

If $\sigma(\alpha)\ne\alpha$, it is another $K$-conjugate and this inequality contradicts the strict hypothesis. Every such automorphism therefore fixes $\alpha$. The [Fundamental theorem of Galois theory](../../../galois-theory.md#fundamental-theorem-of-galois-theory) gives $\alpha\in F$, proving

$$
\boxed{K(\alpha)\subseteq K(\beta).}
$$

Only $\alpha$ needs to be a [separable algebraic element](../../../galois-theory.md#separable-algebraic-element): the proof works even when $\beta$ is inseparable, because the splitting field is taken over $K(\beta)$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Choose compatible primitive [roots of unity](../../../algebra.md#root-of-unity) $\zeta_{p^{n+1}}$, with $\zeta_{p^{n+2}}^p=\zeta_{p^{n+1}}$. Use the slightly faster-converging series permitted by “or otherwise”:

$$
A_N=\sum_{n=0}^Np^{2n}\zeta_{p^{n+1}}.
$$

The terms have [field absolute value](../../../arithmetic.md#absolute-value-algebra) $p^{-2n}$, so the partial sums are a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in $\overline{\mathbb Q}_p$. We show that an algebraic limit would contradict the growth of cyclotomic extension degrees. The faster weights make the strict conjugate-distance estimate work uniformly also at $p=2$.

Put $L_N=\mathbb Q_p(\zeta_{p^{N+1}})$. Its degree is $p^N(p-1)$: the translated [cyclotomic polynomial](../../../galois-theory.md#cyclotomic-polynomial) $\Phi_{p^{N+1}}(1+T)$ has constant term $p$ and reduces modulo $p$ to $T^{p^N(p-1)}$, so is Eisenstein. To verify the reduction, write it as $\sum_{j=0}^{p-1}(1+T)^{jp^N}$ and use characteristic $p$ to reduce this to $\sum_{j=0}^{p-1}(1+T^{p^N})^j=T^{p^N(p-1)}$. All roots lie in $L_N$, and its Galois automorphisms are $\sigma_a(\zeta)=\zeta^a$ for units $a$ modulo $p^{N+1}$.

For a nonidentity automorphism, put $r=v_p(a-1)$, choosing a representative with $0\le r\le N$. It fixes the terms with $n<r$. For $n\ge r$, the root $\zeta_{p^{n+1}}^{a-1}$ has order $p^{n+1-r}$, so the root-of-unity [valuation](../../../algebra.md#valuation) formula, with $v_p(p)=1$, gives

$$
v_p\!\left(p^{2n}(\sigma_a\zeta_{p^{n+1}}-\zeta_{p^{n+1}})\right)=2n+\frac1{p^{n-r}(p-1)}.
$$

This is strictly increasing as $n$ increases: successive differences are $2-p^{-(n-r+1)}>0$. Thus the first changed term is the unique term of smallest [valuation](../../../algebra.md#valuation) and cannot cancel. Consequently

$$
v_p(\sigma_aA_N-A_N)=2r+\frac1{p-1}\le2N+\frac1{p-1}.
$$

In particular no nonidentity automorphism fixes $A_N$, so $\mathbb Q_p(A_N)=L_N$. Also the distance from $A_N$ to every distinct conjugate is at least $p^{-2N-1/(p-1)}$.

Suppose the [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) converged to $A\in\overline{\mathbb Q}_p$. The tail estimate gives

$$
|A-A_N|_p\le p^{-2N-2}<p^{-2N-1/(p-1)}.
$$

Apply [Krasner's lemma](../../../arithmetic.md#krasner-s-lemma) with $\alpha=A_N$, $\beta=A$. It forces $L_N=\mathbb Q_p(A_N)\subseteq\mathbb Q_p(A)$ for every $N$. The right-hand side has finite degree, while $[L_N:\mathbb Q_p]=p^N(p-1)$ is unbounded, a contradiction. Therefore

$$
\boxed{\overline{\mathbb Q}_p\text{ is not complete}.}
$$

This proves [algebraic closure of the p-adic numbers is not complete](../../../arithmetic.md#algebraic-closure-of-the-p-adic-numbers-is-not-complete) by an explicit algebraic [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) and a fully quantified conjugate-separation argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
