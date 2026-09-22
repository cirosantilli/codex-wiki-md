# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper24.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Two [absolute values on a field](../../../arithmetic.md#absolute-value-algebra) are [equivalent absolute values](../../../arithmetic.md#equivalent-absolute-values) when they induce the same [topology](../../../topology.md). For nontrivial [absolute values on a field](../../../arithmetic.md#absolute-value-algebra) this is equivalent to

$$
|x|_2=|x|_1^c\qquad(x\in K)
$$

for a fixed real number $c>0$. The [trivial absolute value](../../../arithmetic.md#trivial-absolute-value) is equivalent only to itself.

Restriction of a [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value) plainly preserves the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality). Conversely, if the restriction is non-Archimedean, every integer, interpreted in either [field](../../../algebra.md#field), has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) at most one. In particular every binomial [coefficient](../../../vector-space.md#coefficient) has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) at most one. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) applied to the binomial expansion gives, for $x,y\in L$ and every positive integer $N$,

$$
|x+y|^N
\leq\sum_{j=0}^N\left|\binom Nj x^j y^{N-j}\right|
\leq (N+1)\max(|x|,|y|)^N.
$$

Raise both sides to the power $1/N$ and let $N\to\infty$. Since $(N+1)^{1/N}\to1$, this yields

$$
\boxed{|x+y|\leq\max(|x|,|y|).}
$$

This is the [bounded-integer criterion for a non-Archimedean absolute value](../../../arithmetic.md#bounded-integer-criterion-for-a-non-archimedean-absolute-value). The proof works for arbitrary [field extensions](../../../algebra.md#field-extension), not just algebraic ones, and in positive characteristic as well.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

First include the [trivial absolute value](../../../arithmetic.md#trivial-absolute-value) if that convention is allowed. For a nontrivial [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value) on $\mathbb Q$, every integer has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) at most one, and some nonzero integer has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) less than one: otherwise every nonzero [rational number](../../../number-theory.md#rational-number), being a quotient of two integers, would have [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) one. Factoring that integer shows that some [prime number](../../../number-theory.md#prime-number) $p$ has $|p|<1$.

There cannot be two such [prime numbers](../../../number-theory.md#prime-number). If $|p|<1$ and $|q|<1$ for distinct [prime numbers](../../../number-theory.md#prime-number), choose integers $a,b$ with $ap+bq=1$. Then the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) gives

$$
1=|1|\leq\max(|a||p|,|b||q|)<1.
$$

Every other [prime number](../../../number-theory.md#prime-number) therefore has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) one. Factoring numerator and denominator of a [rational number](../../../number-theory.md#rational-number) gives

$$
|x|=|p|^{v_p(x)}=|x|_p^c,\qquad
c=\frac{-\log |p|}{\log p}>0.
$$

Thus the nontrivial equivalence classes are precisely the [p-adic absolute values](../../../arithmetic.md#p-adic-absolute-value), one for each [prime number](../../../number-theory.md#prime-number).

Now let $F$ be a [number field](../../../algebraic-number-theory.md#number-field), with [ring of integers of a number field](../../../algebraic-number-theory.md#ring-of-integers) $A$. If the restriction of an [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) to $\mathbb Q$ is trivial, a [monic polynomial](../../../polynomial.md#monic-polynomial) over $\mathbb Q$ satisfied by $x\in F$ forces $|x|\leq1$: if $|x|>1$, its leading term would strictly dominate the other terms. Applying the same argument to $x^{-1}$ forces $|x|=1$ for $x\ne0$. Thus a nontrivial [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) defined on $F$ has a nontrivial restriction, associated with some [prime number](../../../number-theory.md#prime-number) $p$.

Every $a\in A$ has $|a|\leq1$, by applying the same leading-term argument to its monic integral equation. Consequently

$$
\mathfrak p=\{a\in A:|a|<1\}
$$

is a proper [prime ideal](../../../commutative-algebra.md#prime-ideal): it is an ideal by the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality), and $|ab|<1$ with $|a|,|b|\leq1$ implies that at least one factor has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) less than one. It is nonzero because it contains $p$.

The [localization](../../../commutative-algebra.md#localization-of-a-ring) $A_{\mathfrak p}$ lies in the [valuation ring](../../../commutative-algebra.md#valuation-ring) of the [absolute value on a field](../../../arithmetic.md#absolute-value-algebra): a denominator outside $\mathfrak p$ has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) one. Since $A$ is a [Dedekind domain](../../../commutative-algebra.md#dedekind-domain), $A_{\mathfrak p}$ is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring). Choose its [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$. Each $x\in F^\times$ has a unique expression

$$
x=\pi^m u,\qquad m=v_{\mathfrak p}(x),\quad u\in A_{\mathfrak p}^{\times}.
$$

Both $u$ and $u^{-1}$ lie in the [valuation ring](../../../commutative-algebra.md#valuation-ring), so $|u|=1$. Also $\pi$ belongs to its [maximal ideal](../../../commutative-algebra.md#maximal-ideal), hence $|\pi|<1$. Therefore $|x|=|\pi|^{v_{\mathfrak p}(x)}$.

Conversely each nonzero [prime ideal](../../../commutative-algebra.md#prime-ideal) of $A$ gives the [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value) $|x|=c^{v_{\mathfrak p}(x)}$ for any $0<c<1$, using the [discrete valuation](../../../commutative-algebra.md#discrete-valuation) of $A_{\mathfrak p}$. All choices of $c$ are equivalent, and different [prime ideals](../../../commutative-algebra.md#prime-ideal) are distinguished by the elements of $A$ having [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) less than one. We have proved [Non-Archimedean absolute values on a number field](../../../arithmetic.md#non-archimedean-absolute-values-on-a-number-field):

$$
\boxed{\{\text{nontrivial equivalence classes on }F\}
\longleftrightarrow
\{\text{nonzero prime ideals of }\mathcal O_F\}.}
$$

The trivial class is additional when trivial [absolute values on a field](../../../arithmetic.md#absolute-value-algebra) are admitted.

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An extending [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is non-Archimedean by Question 1(a). We prove [finite-dimensional non-Archimedean norm equivalence over a complete field](../../../arithmetic.md#finite-dimensional-non-archimedean-norm-equivalence-over-a-complete-field), using completeness rather than [local compactness](../../../topology.md#locally-compact-space).

Fix a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_d$ of a finite-dimensional [vector space](../../../vector-space.md) over $K$, and let $\|\cdot\|$ be a [norm](../../../functional-analysis.md#norm) homogeneous for the given [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) and satisfying the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality). Write $\|\sum a_i e_i\|_0=\max_i|a_i|$. The upper bound

$$
\|v\|\leq C\|v\|_0,\qquad C=\max_i\|e_i\|,
$$

is immediate. For the lower bound use induction on $d$. The one-dimensional case is homogeneity. For the induction step, the span $W$ of $e_1,\ldots,e_{d-1}$ is complete for its restricted [norm](../../../functional-analysis.md#norm) by the induction comparison with the coordinate [norm](../../../functional-analysis.md#norm) and completeness of $K$. A complete [vector subspace](../../../vector-space.md#vector-subspace) of a [metric space](../../../topological-analysis.md#metric-space) is closed, so

$$
\delta=\inf_{w\in W}\|e_d-w\|>0.
$$

For $v=w+ae_d$ with $a\ne0$, scaling by $a$ gives $\|v\|\geq |a|\delta$; the same [coefficient](../../../vector-space.md#coefficient) bound is trivial when $a=0$. Also

$$
\|w\|\leq\max(\|v\|,|a|\|e_d\|)
\leq\max(1,\delta^{-1}\|e_d\|)\|v\|.
$$

The induction bound controls every coordinate of $w$ by a constant times $\|w\|$. Together with the bound on $a$, this proves $\|v\|_0\leq C'\|v\|$.

Two extending [absolute values on a field](../../../arithmetic.md#absolute-value-algebra) on $L$ are [norms](../../../functional-analysis.md#norm) of this kind on its finite-dimensional [vector space](../../../vector-space.md) over $K$. Hence there is $B>0$ with $|x|_2\leq B|x|_1$ for every $x\in L$. Apply this to $x^N$ and use multiplicativity:

$$
|x|_2\leq B^{1/N}|x|_1.
$$

Letting $N\to\infty$ gives $|x|_2\leq|x|_1$. Interchanging the two [norms](../../../functional-analysis.md#norm) gives equality. Thus

$$
\boxed{\text{There is at most one extending absolute value.}}
$$

The proof covers the trivial base [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) too. It proves uniqueness, without assuming an existence theorem or [compactness](../../../topology.md#compact-space) of the coordinate sphere $\{v:\|v\|_0=1\}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

**False.** This is an example of [integral trace need not imply integrality](../../../algebraic-number-theory.md#integral-trace-need-not-imply-integrality). Take $K=\mathbb Q_p(\theta)$ with $\theta^2=p$, the [splitting field](../../../galois-theory.md#splitting-field) of $X^2-p$. Its two conjugates are $\theta,-\theta$, and its normalized [discrete valuation](../../../commutative-algebra.md#discrete-valuation) satisfies $v_K(\theta)=1$, $v_K(p)=2$, by the [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) criterion. For

$$
x=\frac{\theta}{p}
$$

the [field trace](../../../algebraic-number-theory.md#field-trace) is zero, but $v_K(x)=-1$. Therefore $x$ is not in the [valuation ring](../../../commutative-algebra.md#valuation-ring), despite having integral [field trace](../../../algebraic-number-theory.md#field-trace). Cancellation in a sum of conjugates explains why a [field trace](../../../algebraic-number-theory.md#field-trace) test fails.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**True.** Each element of the [Galois group](../../../galois-theory.md#galois-group) preserves the extending [absolute value on a field](../../../arithmetic.md#absolute-value-algebra), because composing it with that [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) gives another extension, equal to the original by part (a). Thus all conjugates of $x$ have the same [absolute value on a field](../../../arithmetic.md#absolute-value-algebra). Writing $d=[K:\mathbb Q_p]$, the [field norm](../../../algebraic-number-theory.md#field-norm) gives

$$
|N_{K/\mathbb Q_p}(x)|_p
=\prod_{\sigma\in\operatorname{Gal}(K/\mathbb Q_p)}|\sigma x|
=|x|^d.
$$

A [unit](../../../algebra.md#unit-in-a-ring) [field norm](../../../algebraic-number-theory.md#field-norm) has [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) one, forcing $|x|=1$. This means both $x$ and $x^{-1}$ are in the [valuation ring](../../../commutative-algebra.md#valuation-ring), so $x$ is a [unit](../../../algebra.md#unit-in-a-ring).

Equivalently, with normalized [discrete valuations](../../../commutative-algebra.md#discrete-valuation) and [residue degree](../../../arithmetic.md#residue-degree) $f$,

$$
\boxed{v_p(N_{K/\mathbb Q_p}x)=f\,v_K(x)=0
\quad\Longrightarrow\quad v_K(x)=0.}
$$

This is [unit norm detects units in a local extension](../../../algebraic-number-theory.md#unit-norm-detects-units-in-a-local-extension).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

**True.** Put $H=\operatorname{Gal}(K/\mathbb Q_p(\beta))$. Every $\sigma\in H$ fixes $\beta$, permutes the [polynomial](../../../polynomial.md)'s [polynomial roots](../../../polynomial.md#root-of-a-polynomial), and is an isometry by the uniqueness proved in part (a). Therefore

$$
|\beta-\sigma(\alpha_1)|
=|\sigma(\beta-\alpha_1)|
=|\beta-\alpha_1|.
$$

The strict inequalities single out $\alpha_1$ as the unique closest [polynomial root](../../../polynomial.md#root-of-a-polynomial), so $\sigma(\alpha_1)=\alpha_1$ for every $\sigma\in H$. The [Fundamental theorem of Galois theory](../../../galois-theory.md#fundamental-theorem-of-galois-theory) then gives

$$
\boxed{\alpha_1\in K^H=\mathbb Q_p(\beta).}
$$

This [closest-root descent in a Galois extension](../../../arithmetic.md#closest-root-descent-in-a-galois-extension) is the relevant form of [Krasner's lemma](../../../arithmetic.md#krasner-s-lemma). If [polynomial roots](../../../polynomial.md#root-of-a-polynomial) repeat, the strict hypothesis excludes a second occurrence of $\alpha_1$; otherwise the same argument applies unchanged.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

**False.** Use the [polynomial](../../../polynomial.md) $X(X^2-p)$, with [splitting field](../../../galois-theory.md#splitting-field) $K=\mathbb Q_p(\theta)$, $\theta^2=p$, and label the [polynomial roots](../../../polynomial.md#root-of-a-polynomial) $0,\theta,-\theta$. Take $\beta=p\theta$. Then

$$
|\beta|=p^{-3/2},\qquad
|\beta-\theta|=|(p-1)\theta|=p^{-1/2},\qquad
|\beta+\theta|=|(p+1)\theta|=p^{-1/2}.
$$

Both $p-1$ and $p+1$ are [p-adic units](../../../arithmetic.md#p-adic-unit), also when $p=2$. Hence zero is the uniquely closest [polynomial root](../../../polynomial.md#root-of-a-polynomial), but $\beta\notin\mathbb Q_p(0)=\mathbb Q_p$, because $\theta\notin\mathbb Q_p$. The [polynomial](../../../polynomial.md) need not be irreducible in the given setup. The inclusion established by [Krasner's lemma](../../../arithmetic.md#krasner-s-lemma) goes in the direction in part (iii), not its converse.

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [strong form of Hensel lemma](../../../arithmetic.md#strong-form-of-hensel-lemma): for $f\in\mathbb Z_p[T]$ and $a\in\mathbb Z_p$, if

$$
v_p(f(a))>2v_p(f'(a)),
$$

there is a unique [polynomial root](../../../polynomial.md#root-of-a-polynomial) $b$ in the ball $v_p(b-a)>v_p(f'(a))$. In particular, a simple [polynomial root](../../../polynomial.md#root-of-a-polynomial) modulo $p$ lifts uniquely in its residue class. Newton iteration gives $v_p(b-a)=v_p(f(a))-v_p(f'(a))$ when $f(a)\ne0$.

For odd $p\notin\{5,7,13\}$, the sets

$$
\{5x^2:x\in\mathbb F_p\},
\qquad
\{-13-7y^2:y\in\mathbb F_p\}
$$

each have $(p+1)/2$ elements, so they intersect. This gives a zero modulo $p$ with $z=1$. The derivative with respect to $z$ is $26$, nonzero modulo $p$, so [Hensel's lemma](../../../arithmetic.md#hensel-s-lemma) lifts $z$ while holding $x,y$ fixed. This is the elementary proof of [isotropy of nondegenerate ternary quadratic forms over finite fields](../../../linear-algebra.md#isotropy-of-nondegenerate-ternary-quadratic-forms-over-finite-fields) followed by a simple-root lift.

At $p=5$, the residue vector $(0,1,1)$ is a zero, and the derivative $14y$ is nonzero. At $p=13$, use $(3,1,0)$, for which the value is 52 and the derivative $10x=30$ is nonzero modulo 13. Again a single-variable Hensel lift suffices.

At $p=2$, hold $x=2,z=1$ and use $f(Y)=7Y^2+33$. At $Y=1$, $f(1)=40$ has [valuation](../../../algebra.md#valuation) 3, while $f'(1)=14$ has [valuation](../../../algebra.md#valuation) 1. Since $3>2$, the strong Hensel inequality gives a [polynomial root](../../../polynomial.md#root-of-a-polynomial) $y\in\mathbb Z_2$, indeed $y\equiv1\pmod4$. This yields a nonzero solution.

At $p=7$, suppose a nonzero solution exists and scale it so that all coordinates are in $\mathbb Z_7$ and at least one is a [unit](../../../algebra.md#unit-in-a-ring). Reduction modulo 7 gives $z^2=5x^2$. Since 5 is not a square modulo 7, both $x,z$ are divisible by 7. In the original equation their terms are then divisible by 49, so $7y^2$ is divisible by 49 as well, forcing $y$ divisible by 7. This contradicts the normalization. Thus [local isotropy of the five seven thirteen form](../../../linear-algebra.md#local-isotropy-of-the-five-seven-thirteen-form) gives

$$
\boxed{\text{The unique obstructing prime is }p=7.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The intended statement uses a nontrivial [Non-Archimedean absolute value](../../../arithmetic.md#non-archimedean-absolute-value). Under that convention choose $t$ with $0<|t|<1$. A compact neighborhood $C$ of zero contains an open ball of some radius $r>0$. For sufficiently large $N$, $t^N\mathcal O_K$ is contained in that ball. The [valuation ring](../../../commutative-algebra.md#valuation-ring) is closed, so $t^N\mathcal O_K$ is a closed subset of $C$ and is compact. Scaling shows that $\mathcal O_K$ itself is compact.

Its [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $\mathfrak m=\{x:|x|<1\}$ is open. The [residue field](../../../commutative-algebra.md#residue-field) $k=\mathcal O_K/\mathfrak m$ is therefore discrete and compact, hence finite: the open cover by its singleton sets has a finite subcover. Since $\mathfrak m$ has finite index, its complement is a finite union of open cosets. Thus $\mathfrak m$ is also closed and compact.

The continuous [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) attains its maximum on $\mathfrak m$. Nontriviality supplies a nonzero element there, so this maximum is $\rho=|\pi|$ for some $\pi\ne0$, with $0<\rho<1$. If $x\in\mathfrak m$, then $|x/\pi|\leq1$, so $\mathfrak m=\pi\mathcal O_K$.

For arbitrary $x\ne0$, choose the integer $n$ for which $\rho^{n+1}<|x|\leq\rho^n$. Then $\rho<|x/\pi^n|\leq1$. This element cannot lie in $\mathfrak m$, by maximality of $\rho$, so its [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is one. Therefore $|x|=\rho^n$. This proves [discrete valuation from nontrivial local compactness](../../../arithmetic.md#discrete-valuation-from-nontrivial-local-compactness):

$$
\boxed{|K^\times|=\rho^{\mathbb Z},\qquad k\text{ finite}.}
$$

The [nontrivial valuation in the local compactness criterion](../../../arithmetic.md#nontrivial-valuation-in-the-local-compactness-criterion) is essential. If the [trivial absolute value](../../../arithmetic.md#trivial-absolute-value) is admitted, the displayed source claim is false: take $\mathbb Q$ with that [absolute value on a field](../../../arithmetic.md#absolute-value-algebra). It is complete and discrete, hence locally compact, but its [valuation ring](../../../commutative-algebra.md#valuation-ring) and [residue field](../../../commutative-algebra.md#residue-field) are both $\mathbb Q$, which is infinite. The intended nontrivial case has been proved above.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A [local field](../../../arithmetic.md#local-field) is nondiscrete and locally compact. In the non-Archimedean case its [valuation ring](../../../commutative-algebra.md#valuation-ring) is compact by the scaling argument in part (b). Any [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) has a tail in a translate of a compact ball, so has a convergent subsequence; the Cauchy property forces the whole sequence to converge. Thus the [field](../../../algebra.md#field) is complete. Part (b) gives a [discrete valuation](../../../commutative-algebra.md#discrete-valuation), a [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$, and a finite [residue field](../../../commutative-algebra.md#residue-field) $k=\mathbb F_q$, $q=p^f$.

We construct the [coefficient](../../../vector-space.md#coefficient) [field](../../../algebra.md#field) rather than presuming it exists. The [polynomial](../../../polynomial.md) $T^q-T$ has derivative $-1$ in characteristic $p$. Every residue element therefore has a unique [polynomial root](../../../polynomial.md#root-of-a-polynomial) lift by [Hensel's lemma](../../../arithmetic.md#hensel-s-lemma). The set $S$ of these $q$ lifts is a [field](../../../algebra.md#field): qth powers preserve addition and multiplication, so sums and products remain [polynomial root](../../../polynomial.md#root-of-a-polynomial) lifts; a nonzero lift has inverse $a^{q-2}$. Reduction identifies $S$ with $\mathbb F_q$. This is the [finite coefficient field in positive-characteristic local fields](../../../arithmetic.md#finite-coefficient-field-in-positive-characteristic-local-fields).

For $x\in\mathcal O_K$, choose $a_0\in S$ with the same residue, write $x=a_0+\pi x_1$, and repeat with $x_1\in\mathcal O_K$. Completeness gives

$$
x=\sum_{j\ge0}a_j\pi^j,\qquad a_j\in S.
$$

The first nonzero [coefficient](../../../vector-space.md#coefficient) determines the [valuation](../../../algebra.md#valuation), so the expansion is unique. Multiplying an arbitrary [field](../../../algebra.md#field) element by a suitable power of $\pi$ reduces it to this case. Consequently substitution $T\mapsto\pi$ gives a valued-field isomorphism

$$
\boxed{K\cong\mathbb F_{p^f}((T)),\qquad f\ge1.}
$$

Addition and multiplication agree with those of [Laurent series](../../../analysis.md#laurent-series) by convergence, and a nonzero series has a nonzero leading [coefficient](../../../vector-space.md#coefficient), establishing injectivity as well as surjectivity.

Conversely, $\mathbb F_q((T))$ is complete for its T-adic [absolute value on a field](../../../arithmetic.md#absolute-value-algebra). Its [valuation ring](../../../commutative-algebra.md#valuation-ring) $\mathbb F_q[[T]]$ is compact: fixing finitely many [coefficients](../../../vector-space.md#coefficient) gives the finite partitions into balls, and the successive [coefficient](../../../vector-space.md#coefficient) choices realize the [inverse limit](../../../module-theory.md#inverse-limit) of the finite rings $\mathbb F_q[T]/(T^n)$. Equivalently it is the product of countably many finite discrete [coefficient](../../../vector-space.md#coefficient) sets. Thus it is a non-Archimedean [local field](../../../arithmetic.md#local-field). Distinct $q$ give nonisomorphic valued [fields](../../../algebra.md#field) because their [residue fields](../../../commutative-algebra.md#residue-field) have different sizes. Replacing $|T|$ by any number in $(0,1)$ gives an equivalent [absolute value on a field](../../../arithmetic.md#absolute-value-algebra).

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $f=[k_L:k]$. For an [unramified extension](../../../arithmetic.md#unramified-extension) the [ramification index](../../../arithmetic.md#ramification-index) is one and $[L:K]=f$. The residue $\bar\alpha$ has degree $f$ over $k$. Thus $1,\alpha,\ldots,\alpha^{f-1}$ are linearly independent over $K$: a nonzero [linear dependence](../../../vector-space.md#linear-dependence) can be divided by a [coefficient](../../../vector-space.md#coefficient) of least [valuation](../../../algebra.md#valuation) and reduced to a nonzero relation among the reduced powers. Hence $[K(\alpha):K]\ge f=[L:K]$, and $\alpha$ generates $L$.

The same argument gives the integral statement, which is stronger than merely generating the [field](../../../algebra.md#field). Write

$$
x=\sum_{j=0}^{f-1}c_j\alpha^j,\qquad c_j\in K.
$$

If $m=\min_j v_K(c_j)$, divide by $\pi_K^m$. Since $\pi_K$ remains a [uniformizer](../../../commutative-algebra.md#uniformizer) in the [unramified extension](../../../arithmetic.md#unramified-extension) and the reduced powers form a [basis](../../../vector-space.md#basis) of $k_L/k$, the resulting sum has nonzero residue. Therefore $v_L(x)=m$. In particular $x$ is integral if and only if every [coefficient](../../../vector-space.md#coefficient) is integral. This proves [unramified residue generator integral basis](../../../arithmetic.md#unramified-residue-generator-integral-basis):

$$
\boxed{\mathcal O_L=\bigoplus_{j=0}^{f-1}\mathcal O_K\alpha^j
=\mathcal O_K[\alpha].}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For the finite [separable field extension](../../../galois-theory.md#separable-extension) define the [inverse different](../../../arithmetic.md#inverse-different), or [codifferent](../../../arithmetic.md#inverse-different), by

$$
\mathfrak D_{L/K}^{-1}
=\{x\in L:\operatorname{Tr}_{L/K}(x\mathcal O_L)
\subseteq\mathcal O_K\}.
$$

It is a [fractional ideal](../../../commutative-algebra.md#fractional-ideal) of $\mathcal O_L$. The [different ideal](../../../arithmetic.md#different-ideal) is its inverse [fractional ideal](../../../commutative-algebra.md#fractional-ideal).

Suppose the integer ring is generated by $\alpha$, with monic [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) $g$ of degree $d$. We prove the derivative formula using the [coefficient pairing for a monogenic algebra](../../../algebraic-number-theory.md#coefficient-pairing-for-a-monogenic-algebra). If $\alpha_1,\ldots,\alpha_d$ are its distinct conjugate [polynomial roots](../../../polynomial.md#root-of-a-polynomial), [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) for a [polynomial](../../../polynomial.md) $h$ of degree less than $d$ gives

$$
h(T)=\sum_{i=1}^d h(\alpha_i)
\frac{g(T)}{(T-\alpha_i)g'(\alpha_i)}.
$$

Comparing [coefficients](../../../vector-space.md#coefficient) of $T^{d-1}$ yields

$$
\operatorname{Tr}_{L/K}\!\left(\frac{h(\alpha)}{g'(\alpha)}\right)
=[T^{d-1}]h(T).
$$

For any integral [polynomial](../../../polynomial.md), first reduce modulo $g$; the [coefficients](../../../vector-space.md#coefficient) stay integral because $g$ is monic over $\mathcal O_K$.

It follows that $g'(\alpha)^{-1}\mathcal O_L$ lies in the [codifferent](../../../arithmetic.md#inverse-different). To prove equality, consider the [matrix](../../../vector-space.md#matrix)

$$
A_{ij}=\operatorname{Tr}_{L/K}
\left(\frac{\alpha^{i+j}}{g'(\alpha)}\right),
\qquad 0\le i,j\le d-1.
$$

All entries are integral. Entries with $i+j<d-1$ are zero, and those with $i+j=d-1$ are one. Reversing the column order makes the [matrix](../../../vector-space.md#matrix) triangular with diagonal ones; thus its [determinant](../../../linear-algebra.md#determinant) is a [unit](../../../algebra.md#unit-in-a-ring) of $\mathcal O_K$.

Write an arbitrary $x\in L$ as $x=g'(\alpha)^{-1}\sum_j b_j\alpha^j$ with $b_j\in K$. Membership in the [codifferent](../../../arithmetic.md#inverse-different) says $A(b_j)_j\in\mathcal O_K^d$. Since $A$ is invertible over $\mathcal O_K$, this forces every $b_j$ integral. Therefore

$$
\mathfrak D_{L/K}^{-1}=g'(\alpha)^{-1}\mathcal O_L,
\qquad
\boxed{\mathfrak D_{L/K}=(g'(\alpha)).}
$$

Separability ensures that $g'(\alpha)\ne0$; the [trace pairing](../../../algebraic-number-theory.md#trace-pairing) calculation also proves that no extra factor has been overlooked.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $L=\mathbb Q_p(\zeta_p)$, put $\pi=\zeta_p-1$. The [polynomial](../../../polynomial.md)

$$
\Phi_p(1+T)=\frac{(1+T)^p-1}{T}
$$

is [Eisenstein](../../../commutative-algebra.md#eisenstein-criterion) at $p$. It gives $[L:\mathbb Q_p]=e=p-1$, total ramification, and $v_L(\pi)=1$. Also $\mathcal O_L=\mathbb Z_p[\pi]$: in the power [basis](../../../vector-space.md#basis), terms $c_i\pi^i$ have [valuations](../../../algebra.md#valuation) $(p-1)v_p(c_i)+i$ in different residue classes modulo $p-1$, so cannot cancel at the minimum. Integrality forces all $c_i$ integral.

Use part (b) with $\Phi_p(T)$ and differentiate the quotient at $\zeta_p$:

$$
\Phi'_p(\zeta_p)=\frac{p\zeta_p^{p-1}}{\zeta_p-1}.
$$

The [root of unity](../../../algebra.md#root-of-unity) is a [unit](../../../algebra.md#unit-in-a-ring), while $v_L(p)=p-1$ and $v_L(\pi)=1$. Hence the [cyclotomic local different exponent](../../../arithmetic.md#cyclotomic-local-different-exponent) is

$$
\boxed{\delta(\mathbb Q_p(\zeta_p)/\mathbb Q_p)=p-2.}
$$

This includes $p=2$: that extension is trivial and the exponent is zero.

For $m=p^2-1$, construct an unramified quadratic extension $E/\mathbb Q_p$ by lifting an irreducible [quadratic polynomial](../../../polynomial.md#quadratic-polynomial) over $\mathbb F_p$. Its [residue field](../../../commutative-algebra.md#residue-field) is $\mathbb F_{p^2}$. Each of its nonzero residue elements is a simple [polynomial root](../../../polynomial.md#root-of-a-polynomial) of $T^m-1$, so [Hensel's lemma](../../../arithmetic.md#hensel-s-lemma) lifts all $m$ [polynomial roots](../../../polynomial.md#root-of-a-polynomial) into $E$. A primitive residue element lifts to a primitive mth [polynomial root](../../../polynomial.md#root-of-a-polynomial): its reduction already has order $m$, and its mth power is one.

Such a primitive [polynomial root](../../../polynomial.md#root-of-a-polynomial) cannot generate a proper subfield of $E$, since its residue has order $p^2-1>p-1$ and therefore generates the quadratic residue extension. Thus $\mathbb Q_p(\zeta_m)=E$ is unramified of degree two. Part (a) gives $\mathcal O_E=\mathbb Z_p[\zeta_m]$. The reduced [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) has degree two and is separable, so its derivative at $\zeta_m$ is a [unit](../../../algebra.md#unit-in-a-ring). Part (b) gives

$$
\boxed{\delta(\mathbb Q_p(\zeta_{p^2-1})/\mathbb Q_p)=0.}
$$

Both answers use normalized [discrete valuations](../../../commutative-algebra.md#discrete-valuation) on the top [field](../../../algebra.md#field).

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $L/K$ be a finite [Galois extension](../../../galois-theory.md#finite-galois-extension) of non-Archimedean [local fields](../../../arithmetic.md#local-field), with [Galois group](../../../galois-theory.md#galois-group) $G$, normalized [valuation](../../../algebra.md#valuation) $v_L$, integer ring $\mathcal O_L$, and residue characteristic $p$. The [lower ramification numbering](../../../arithmetic.md#lower-ramification-numbering) is

$$
G_{-1}=G,\qquad
G_i=\{\sigma\in G:v_L(\sigma a-a)\ge i+1
\text{ for every }a\in\mathcal O_L\},\quad i\ge0.
$$

These [higher ramification groups](../../../arithmetic.md#ramification-group) measure successively finer agreement with the identity. The [group](../../../group.md) $G_0$ is the [inertia group](../../../arithmetic.md#inertia-group), the kernel of the action on the [residue field](../../../commutative-algebra.md#residue-field). Each $G_i$ is normal in $G$: conjugation permutes integral elements and preserves their [valuations](../../../algebra.md#valuation). The [groups](../../../group.md) eventually become trivial, since each nonidentity automorphism moves some integral element and its displacement has finite [valuation](../../../algebra.md#valuation).

Let $K_0=L^{G_0}$, the [maximal unramified subextension of a local field extension](../../../arithmetic.md#maximal-unramified-subextension-of-a-local-field-extension). Then $G/G_0$ is the [Galois group](../../../galois-theory.md#galois-group) of the residue extension, cyclic and generated by a [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism). For a [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$ of $L$, the [uniformizer criterion for lower ramification groups](../../../arithmetic.md#uniformizer-criterion-for-lower-ramification-groups) gives

$$
G_i=\{\sigma\in G_0:v_L(\sigma\pi-\pi)\ge i+1\}.
$$

To see why one [uniformizer](../../../commutative-algebra.md#uniformizer) suffices, the extension $L/K_0$ is totally ramified and its integer ring is $\mathcal O_{K_0}[\pi]$. Elements of $G_0$ fix its [coefficients](../../../vector-space.md#coefficient). Differences of powers of $\pi$ are divisible by $\sigma\pi-\pi$, so the [valuation](../../../algebra.md#valuation) bound for $\pi$ implies it for every integral element. The converse follows by testing $\pi$ itself.

The [tame inertia quotient](../../../arithmetic.md#tame-inertia-quotient) is seen explicitly from

$$
G_0\longrightarrow k_L^\times,\qquad
\sigma\longmapsto\overline{\sigma\pi/\pi}.
$$

It is a homomorphism because inertia acts trivially on the [residue field](../../../commutative-algebra.md#residue-field), and its kernel is $G_1$. Thus $G_0/G_1$ is cyclic of order not divisible by $p$. For $i\ge1$, the homomorphism

$$
G_i\longrightarrow(k_L,+),\qquad
\sigma\longmapsto
\overline{\frac{\sigma\pi-\pi}{\pi^{i+1}}}
$$

has kernel $G_{i+1}$. Indeed composing two automorphisms adds the leading displacements, since $\sigma\pi/\pi\equiv1$ and inertia fixes residue [coefficients](../../../vector-space.md#coefficient). Hence each $G_i/G_{i+1}$ is an [elementary abelian p-group](../../../group.md#elementary-abelian-group). Eventual triviality makes $G_1$ a [p-group](../../../finite-group-theory.md#p-group); the prime-to-p quotient makes it the unique [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $G_0$. This is the [wild inertia group](../../../arithmetic.md#wild-inertia-group). [Tame ramification](../../../arithmetic.md#tamely-ramified-extension) means $G_1=1$.

The filtration also measures the [different exponent](../../../arithmetic.md#different-exponent). For the [totally ramified extension](../../../arithmetic.md#totally-ramified-extension) over $K_0$, the [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) $g$ of $\pi$ has [polynomial roots](../../../polynomial.md#root-of-a-polynomial) $\sigma\pi$, $\sigma\in G_0$. The derivative formula gives

$$
v_L(g'(\pi))=\sum_{\sigma\in G_0\setminus\{1\}}
v_L(\pi-\sigma\pi).
$$

For a fixed $\sigma$, its displacement [valuation](../../../algebra.md#valuation) is the number of indices $i\ge0$ for which it belongs to $G_i$. Interchanging the finite sums therefore gives [different exponent from ramification groups](../../../arithmetic.md#different-exponent-from-ramification-groups):

$$
\boxed{\delta(L/K)=\sum_{i\ge0}(|G_i|-1).}
$$

The unramified part contributes zero. More generally [different in a tower](../../../arithmetic.md#different-in-a-tower) follows by taking products of [bases of a module](../../../module-theory.md#basis-of-a-module) dual for the [trace pairing](../../../algebraic-number-theory.md#trace-pairing), and gives

$$
\delta(L/K)=\delta(L/E)+e(L/E)\delta(E/K).
$$

Thus a tame extension has [different exponent](../../../arithmetic.md#different-exponent) $e-1$, while nontrivial wild [groups](../../../group.md) contribute additional positive terms.

The lower numbering restricts to [subgroups](../../../group.md#subgroup): if $H=\operatorname{Gal}(L/E)$, its [groups](../../../group.md) are $H_i=H\cap G_i$, directly from the definition using the same top-field [valuation](../../../algebra.md#valuation). Quotients need a different indexing. For real $s\ge0$ put $G_s=G_{\lceil s\rceil}$ and define the [Herbrand function](../../../arithmetic.md#herbrand-function)

$$
\varphi(s)=\int_0^s\frac{dt}{[G_0:G_t]},\qquad
\psi=\varphi^{-1},\qquad G^u=G_{\psi(u)}.
$$

This [upper ramification numbering](../../../arithmetic.md#upper-ramification-numbering) stretches or compresses intervals according to the inertia indices. The quotient theorem says that for a [normal subgroup](../../../group-theory.md#normal-subgroup) $H$, [upper ramification groups commute with quotients](../../../arithmetic.md#upper-ramification-groups-commute-with-quotients):

$$
(G/H)^u=G^uH/H.
$$

In particular the same upper index has a meaning compatible with passing to a smaller [Galois extension](../../../galois-theory.md#finite-galois-extension), which lower indices generally lack.

For a tame [totally ramified extension](../../../arithmetic.md#totally-ramified-extension) the picture is simple: $G_0=G$, all $G_i$ with $i\ge1$ are trivial, and the [different exponent](../../../arithmetic.md#different-exponent) is $|G|-1$. The extension $\mathbb Q_p(\zeta_p)$ for odd $p$ illustrates this, giving exponent $p-2$.

A mixed-characteristic wild family is the [lower ramification filtration of a prime-power cyclotomic extension](../../../arithmetic.md#lower-ramification-filtration-of-a-prime-power-cyclotomic-extension). Take $L=\mathbb Q_p(\zeta_{p^r})$ with odd $p$ and $\pi=\zeta_{p^r}-1$. If $\sigma_a(\zeta)=\zeta^a$ and $a\ne1$ modulo $p^r$, then

$$
v_L(\sigma_a\pi-\pi)
=v_L(\zeta^{a-1}-1)=p^{v_p(a-1)}.
$$

The last equality follows because $\zeta^{a-1}$ has order $p^{r-v_p(a-1)}$ and its [uniformizer](../../../commutative-algebra.md#uniformizer) [valuation](../../../algebra.md#valuation) scales by the [ramification index](../../../arithmetic.md#ramification-index) in that cyclotomic tower. The lower breaks are $0,p-1,p^2-1,\ldots,p^{r-1}-1$. Integrating the successive indices $(p-1),p(p-1),\ldots$ gives upper breaks $0,1,\ldots,r-1$.

In equal characteristic there is an equally explicit wild example. Start with $K=\mathbb F_q((t))$ and an [Artin–Schreier extension](../../../galois-theory.md#artin-schreier-extension)

$$
y^p-y=t^{-m},\qquad m>0,\quad p\nmid m.
$$

There is no [polynomial root](../../../polynomial.md#root-of-a-polynomial) in $K$: a negative-valuation element has $v(x^p-x)=p\,v(x)$, while the right side has [valuation](../../../algebra.md#valuation) $-m$. Adjoining a [polynomial root](../../../polynomial.md#root-of-a-polynomial) splits the [polynomial](../../../polynomial.md), whose [polynomial roots](../../../polynomial.md#root-of-a-polynomial) are $y+c$ for $c\in\mathbb F_p$, so the extension is cyclic of degree $p$. The [valuation](../../../algebra.md#valuation) equation forces total ramification, $v_L(t)=p$ and $v_L(y)=-m$. Choose $1\le b\le p-1$ with $-bm\equiv1\pmod p$ and set $a=(1+bm)/p$. Then $\pi=t^a y^b$ is a [uniformizer](../../../commutative-algebra.md#uniformizer). For a nonidentity automorphism $y\mapsto y+c$,

$$
\frac{\sigma\pi}{\pi}=(1+c/y)^b,\qquad
v_L(\sigma\pi-\pi)=1+m;
$$

the first [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $b$ is nonzero modulo $p$, and all subsequent terms have strictly higher [valuation](../../../algebra.md#valuation). Therefore

$$
G_0=\cdots=G_m=C_p,\qquad G_{m+1}=1,\qquad
\delta=(m+1)(p-1).
$$

This is the [ramification break of an Artin–Schreier pole](../../../arithmetic.md#ramification-break-of-an-artin-schreier-pole). It shows concretely that wild breaks, unlike tame inertia, can occur arbitrarily far out in the filtration.

**The lower [groups](../../../group.md) measure integral displacements, the upper [groups](../../../group.md) make quotient comparison possible, and the sizes of the [groups](../../../group.md) determine the different.**

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [polynomial](../../../polynomial.md) is [Eisenstein](../../../commutative-algebra.md#eisenstein-criterion) at every [prime number](../../../number-theory.md#prime-number) $p$, so a [polynomial root](../../../polynomial.md#root-of-a-polynomial) $\alpha$ generates a totally ramified cubic [field](../../../algebra.md#field) $F/\mathbb Q_p$. The splitting-field [Galois group](../../../galois-theory.md#galois-group) is a transitive [subgroup](../../../group.md#subgroup) of $S_3$, hence $C_3$ or $S_3$. Its [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is

$$
\Delta=-p^2(4p+27).
$$

The product of the three [polynomial root](../../../polynomial.md#root-of-a-polynomial) differences is a [square root](../../../algebra.md#square-root) of $\Delta$, transformed by the sign of the [polynomial root](../../../polynomial.md#root-of-a-polynomial) permutation. Thus the [group](../../../group.md) is $C_3$ exactly when $\Delta$ is a square, and otherwise it is $S_3$. In the latter case the [splitting field](../../../galois-theory.md#splitting-field) is

$$
L=F\,\mathbb Q_p(\sqrt{\Delta}).
$$

Indeed adjoining one [polynomial root](../../../polynomial.md#root-of-a-polynomial) leaves a quadratic factor, whose [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is $\Delta/f'(\alpha)^2$, so the [square root](../../../algebra.md#square-root) of $\Delta$ supplies its remaining [polynomial roots](../../../polynomial.md#root-of-a-polynomial).

Suppose first that $p>3$. The [unit](../../../algebra.md#unit-in-a-ring) $-(4p+27)$ reduces to $-27$, and [Hensel's lemma](../../../arithmetic.md#hensel-s-lemma) makes it a square exactly when $-3$ is a square modulo $p$. [Quadratic reciprocity](../../../number-theory.md#quadratic-reciprocity) gives

$$
\left(\frac{-3}{p}\right)=
\begin{cases}1,&p\equiv1\pmod3,\\-1,&p\equiv2\pmod3.\end{cases}
$$

If $p\equiv1\pmod3$, the [field](../../../algebra.md#field) generated by $\alpha$ is already the cyclic [splitting field](../../../galois-theory.md#splitting-field), totally ramified of degree three. If $p\equiv2\pmod3$, the nonsquare [unit](../../../algebra.md#unit-in-a-ring) gives an unramified quadratic [field](../../../algebra.md#field) $E=\mathbb Q_p(\sqrt{\Delta})$. Since $F$ and $E$ have coprime degrees, $[FE:\mathbb Q_p]=6$. Its [residue degree](../../../arithmetic.md#residue-degree) is at least two and its [ramification index](../../../arithmetic.md#ramification-index) at least three; their product is six, so they are exactly two and three. Thus its [inertia group](../../../arithmetic.md#inertia-group) is the normal $C_3$ inside $S_3$.

In both cases the [ramification index](../../../arithmetic.md#ramification-index) is three and is not divisible by $p$. The [wild inertia group](../../../arithmetic.md#wild-inertia-group) is trivial, so all positive lower [groups](../../../group.md) are trivial. As a different check, $f'(\alpha)=3\alpha^2+p$ has [valuation](../../../algebra.md#valuation) two in $F$ when $p>3$, agreeing with tame [different exponent](../../../arithmetic.md#different-exponent) $3-1$.

For $p=3$ the [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is $-351=-3^3\cdot13$, which is nonsquare. Hence $G=S_3$. The quadratic subfield can be written $E=\mathbb Q_3(\beta)$ with $\beta^2=-39$. It is ramified of degree two, by the [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) $T^2+39$. Together with the totally ramified cubic [field](../../../algebra.md#field) this forces $e(L/\mathbb Q_3)$ to be divisible by both two and three. Since $[L:\mathbb Q_3]=6$, the [splitting field](../../../galois-theory.md#splitting-field) is totally ramified. In its normalized [valuation](../../../algebra.md#valuation),

$$
v_L(3)=6,\quad v_L(\alpha)=2,\quad
v_L(\beta)=3,\quad \pi=\beta/\alpha\text{ has }v_L(\pi)=1.
$$

All differences between distinct [polynomial roots](../../../polynomial.md#root-of-a-polynomial) have the same [valuation](../../../algebra.md#valuation), since $S_3$ permutes the [polynomial root](../../../polynomial.md#root-of-a-polynomial) pairs and preserves the [absolute value on a field](../../../arithmetic.md#absolute-value-algebra). Also

$$
f'(\alpha)=3(\alpha^2+1)
=(\alpha-\alpha_2)(\alpha-\alpha_3)
$$

has [valuation](../../../algebra.md#valuation) six, so each [polynomial root](../../../polynomial.md#root-of-a-polynomial) difference has [valuation](../../../algebra.md#valuation) three. A nonidentity [three-cycle](../../../finite-group-theory.md#three-cycle) fixes $\beta$, and therefore

$$
v_L(\sigma\pi-\pi)
=v_L\left(\frac{\beta(\alpha-\sigma\alpha)}
{\alpha\,\sigma\alpha}\right)
=3+3-2-2=2.
$$

The [transposition](../../../combinatorics.md#transposition-permutation) fixing $\alpha$ negates $\beta$, so sends $\pi$ to $-\pi$ and has displacement [valuation](../../../algebra.md#valuation) $v_L(2\pi)=1$. The other [transpositions](../../../combinatorics.md#transposition-permutation) have the same value by conjugacy. The [uniformizer](../../../commutative-algebra.md#uniformizer) criterion now determines every [group](../../../group.md):

$$
\boxed{
\begin{array}{c|c|c|c|c}
p&G&e&f&(G_0,G_1,G_2,\ldots)\\
p>3,\ p\equiv1\pmod3&C_3&3&1&(C_3,1,1,\ldots)\\
p>3,\ p\equiv2\pmod3&S_3&3&2&(C_3,1,1,\ldots)\\
p=3&S_3&6&1&(S_3,C_3,1,1,\ldots)
\end{array}}
$$

For the wild case the [different exponent](../../../arithmetic.md#different-exponent) is $5+2=7$. Independently, the cubic subfield has [different exponent](../../../arithmetic.md#different-exponent) $v_F(3(\alpha^2+1))=3$, and the quadratic extension $L/F$ is tame with exponent one. The tower formula gives $1+2\cdot3=7$, confirming the filtration. Its positive upper break is $1/2$, because $[G_0:G_1]=2$. This completes [ramification of the splitting field of X3 plus pX plus p](../../../arithmetic.md#ramification-of-the-splitting-field-of-x3-plus-px-plus-p) for every odd [prime number](../../../number-theory.md#prime-number).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
