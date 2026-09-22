# Prime number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_number)

A [prime number](prime-number.md) is a [positive integer](integer.md#positive-integer) $p>1$ whose only positive [divisors](divisibility.md#divisor) are $1$ and $p$. The first ten [prime numbers](prime-number.md) are $2,3,5,7,11,13,17,19,23,29$. In contrast, $12=3\cdot4$ is a [composite number](number-theory.md#composite-number) because it has a positive [divisor](divisibility.md#divisor) strictly between one and itself. The [integer](integer.md) one is neither a [prime number](prime-number.md) nor a [composite number](number-theory.md#composite-number): the lower bound $p>1$ is part of the definition. Equivalently, the [divisor function](arithmetic-function.md#divisor-function) satisfies $\tau(p)=2$ for a [prime number](prime-number.md), whereas $\tau(1)=1$ and $\tau(n)\geq3$ for every [composite number](number-theory.md#composite-number) $n$.

[Prime numbers](prime-number.md) are the building blocks of [positive integers](integer.md#positive-integer) under [multiplication](arithmetic.md#multiplication). The [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic) says that every [integer](integer.md) greater than one is a [product](arithmetic.md#product-of-numbers) of [prime numbers](prime-number.md), with a unique collection of factors when their order is ignored. For example, $12=2\cdot2\cdot3$ and $18=2\cdot3\cdot3$. Their common factors reveal the [greatest common divisor](divisibility.md#greatest-common-divisor) $6$, and the combined maximum powers reveal the [least common multiple](divisibility.md#least-common-multiple) $36$. A complicated [divisibility](divisibility.md) question becomes a comparison of prime exponents.

There is also a useful finite test. If a [composite number](number-theory.md#composite-number) $n$ equals $ab$ with $1<a\leq b$, then $a^2\leq n$. Therefore some [prime factor](#prime-factor) is at most $\sqrt n$, and [trial division](#trial-division) only needs to check [prime numbers](prime-number.md) up to that [square root](algebra.md#square-root). For $97$, checking $2,3,5,7$ suffices; none divides $97$, so it is a [prime number](prime-number.md). For $91$, the same test finds $7$, giving $91=7\cdot13$. To find many [prime numbers](prime-number.md) together, the [sieve of Eratosthenes](#sieve-of-eratosthenes) reuses the work by marking multiples.

The [division with remainder](integer.md#euclidean-division) calculations for $97$ make the test explicit:

$$
97=2\cdot48+1=3\cdot32+1=5\cdot19+2=7\cdot13+6.
$$

Since $9^2<97<10^2$, these are all the [prime numbers](prime-number.md) at most its [square root](algebra.md#square-root), and every [remainder](integer.md#remainder) is nonzero. Thus the calculation certifies a [prime number](prime-number.md), without testing the [integers](integer.md) $8,9,10,\ldots,96$ individually. In contrast, $91=7\cdot13+0$ gives a [prime factor](#prime-factor) and proves that $91$ is a [composite number](number-theory.md#composite-number).

The definition has a long history. Book VII of [Euclid's Elements](euclidean-geometry.md#euclid-s-elements) distinguishes [prime numbers](prime-number.md) from [composite numbers](number-theory.md#composite-number) through their possible measures; Book IX, Proposition 20 establishes that no finite list exhausts the [prime numbers](prime-number.md). The modern argument under [Euclid's theorem](#euclid-s-theorem) needs only [divisibility](divisibility.md), so it proves an infinite conclusion without estimating how frequently [prime numbers](prime-number.md) occur. [Euclid, Elements, Book VII, definitions 11–14, David Joyce's edition](https://mathcs.clarku.edu/~djoyce/elements/bookVII/defVII11.html) [Euclid, Elements, Book IX, Proposition 20](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX20.html).

**Table of contents**

- [Prime gap](#prime-gap)
- [Prime constellation](#prime-constellation)
- [Prime quadruplet](#prime-quadruplet)
- [Sexy prime pair](#sexy-prime-pair)
- [Cuban prime](#cuban-prime)
- [Truncatable prime](#truncatable-prime)
- [Circular prime](#circular-prime)
- [Primality](#primality)
- [Trial division](#trial-division)
- [Sieve of Eratosthenes](#sieve-of-eratosthenes)
- [Infinitely many primes congruent to one modulo six](#infinitely-many-primes-congruent-to-one-modulo-six)
- [Infinitely many primes congruent to minus one modulo six](#infinitely-many-primes-congruent-to-minus-one-modulo-six)
- [Bertrand's postulate](#bertrand-s-postulate)
- [Twin prime](#twin-prime)
  - [Twin prime conjecture](#twin-prime-conjecture)
    - [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture)
    - [Twin-prime constant](#twin-prime-constant)
  - [Brun's theorem](#brun-s-theorem)
  - [Twin-prime upper bound using Bombieri–Vinogradov](#twin-prime-upper-bound-using-bombieri-vinogradov)
- [Euclid's theorem](#euclid-s-theorem)
- [Odd prime](#odd-prime)
- [Fermat prime](#fermat-prime)
  - [Pépin's test](#pepin-s-test)
  - [Quadratic nonresidues modulo a Fermat prime](#quadratic-nonresidues-modulo-a-fermat-prime)
- [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)
  - [Prime signature](#prime-signature)
  - [Factorization tree](#factorization-tree)
- [Prime factor](#prime-factor)
  - [Smallest prime factor](#smallest-prime-factor)
- [Prime power](#prime-power)

## Prime gap

↑ **Parent:** [Prime number](prime-number.md)

## Prime constellation

↑ **Parent:** [Prime number](prime-number.md)

## Prime quadruplet

↑ **Parent:** [Prime number](prime-number.md)

A prime quadruplet is a set of four [primes](prime-number.md) $p,p+2,p+6,p+8$. For example, $5,7,11,13$ form a prime quadruplet. Testing candidates uses [integer congruences](modular-arithmetic.md#integer-congruence) to discard starting values for which one of the four entries has a small [prime factor](#prime-factor).

## Sexy prime pair

↑ **Parent:** [Prime number](prime-number.md)

Two [primes](prime-number.md) whose difference is $6$, for example $5$ and $11$. The name refers to the Latin word for six. The [primes](prime-number.md) need not be consecutive.

## Cuban prime

↑ **Parent:** [Prime number](prime-number.md)

A [prime number](prime-number.md) expressible as $(x^3-y^3)/(x-y)=x^2+xy+y^2$ for specified consecutive or nearly consecutive [positive integers](integer.md#positive-integer). The first kind has $x=y+1$ and therefore the form $3y^2+3y+1$; the second kind has $x=y+2$ and therefore the form $3y^2+6y+4$. The first kind arises when a [difference of two cubes](polynomial.md#difference-of-two-cubes) is itself [prime](prime-number.md): the factorization $x^3-y^3=(x-y)(x^2+xy+y^2)$ forces $x-y=1$ for $x>y>0$.

## Truncatable prime

↑ **Parent:** [Prime number](prime-number.md)

A [prime number](prime-number.md) that remains [prime](prime-number.md) after successively deleting digits from a specified end of its [positional notation](integer.md#positional-notation). Left truncation, right truncation, and requiring both are distinct conditions. For example, $3797$ is truncatable from both ends: $3797,797,97,7$ and $3797,379,37,3$ consist entirely of [prime numbers](prime-number.md).

## Circular prime

↑ **Parent:** [Prime number](prime-number.md)

A [prime number](prime-number.md) for which every cyclic rotation of its [numerical digits](integer.md#numerical-digit) is also a [prime number](prime-number.md). In [decimal representation](integer.md#decimal-representation), $197$ is an example because $197,971,719$ are all [prime numbers](prime-number.md). A multi-digit [circular prime](#circular-prime) can contain only $1,3,7,9$: any other digit can be rotated into the units position and force [divisibility](divisibility.md) by $2$ or $5$.

## Primality

↑ **Parent:** [Prime number](prime-number.md)

[Primality](#primality) is the property of a [positive integer](integer.md#positive-integer) being a [prime number](prime-number.md). [Primality testing](theoretical-computer-science.md#primality-testing) determines this property; [integer factorization](number-theory.md#integer-factorization) asks for factors and is a different computational task.

## Trial division

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trial_division)

[Trial division](#trial-division) searches for [divisors](divisibility.md#divisor) of an [integer](integer.md) by testing candidate divisions. For [primality testing](theoretical-computer-science.md#primality-testing) of an [integer](integer.md) $n>1$, testing the [prime numbers](prime-number.md) up to $\sqrt n$ suffices: any [composite number](number-theory.md#composite-number) has a [prime factor](#prime-factor) in that range. After finding a [prime factor](#prime-factor), repeated [division](arithmetic.md#division-mathematics) removes its [prime power](#prime-power), and testing the remaining quotient gives an elementary [integer factorization](number-theory.md#integer-factorization) method. This is useful for small inputs, but the number of candidates can grow rapidly with the input's digit count.

## Sieve of Eratosthenes

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes)

The [sieve of Eratosthenes](#sieve-of-eratosthenes) finds all [prime numbers](prime-number.md) at most an [integer](integer.md) $N\geq2$. Start with the [integers](integer.md) $2,\ldots,N$ marked as candidates. For each surviving candidate $p$ in increasing order, mark the multiples $p^2,p^2+p,\ldots$ up to $N$ as [composite numbers](number-theory.md#composite-number). Stop processing candidates once $p^2>N$: the surviving candidates are exactly the [prime numbers](prime-number.md). Starting at $p^2$ saves work because any smaller proper multiple of $p$ already has a smaller [prime factor](#prime-factor). [Jerry Cain, Stanford CS106AJ, Section Handout 6, Problem 4: the sieve of Eratosthenes](https://web.stanford.edu/class/cs106aj/res/handouts/36-Section-6.pdf).

For a complete run with $N=60$, the only [prime numbers](prime-number.md) at most $\sqrt{60}$ are $2,3,5,7$, since $7^2\leq60<8^2$. Exclude one before starting; it is not a [prime number](prime-number.md). The four marking passes are:
- $p=2$: mark $4,6,8,\ldots,60$, removing 29 candidates.
- $p=3$: mark $9,12,15,\ldots,60$. The nine newly removed candidates are $9,15,21,27,33,39,45,51,57$; the [even integers](integer.md#even-number) were already marked.
- $p=5$: mark $25,30,35,40,45,50,55,60$. Only $25,35,55$ are newly removed.
- $p=7$: mark $49,56$. Only $49$ is newly removed.

There are $59-29-9-3-1=17$ surviving [prime numbers](prime-number.md):

$$
2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59.
$$

The next surviving candidate is $11$, and $11^2>60$, so no further marking pass is necessary. A [prime number](prime-number.md) used for marking remains a candidate: starting at $p^2$ never marks $p$ itself.

<a id="image-four-passes-of-the-sieve-of-eratosthenes-through-60-leave-seventeen-prime-numbers"></a>
![](prime-sieve-steps.png)

**[Figure 1](#image-four-passes-of-the-sieve-of-eratosthenes-through-60-leave-seventeen-prime-numbers). Four passes of the sieve of Eratosthenes through 60 leave seventeen prime numbers**. Blue cells are newly marked [composite numbers](number-theory.md#composite-number); gray cells were removed earlier. White cells are candidates in the first three panels, and green cells are the final [prime numbers](prime-number.md). The outlined cell identifies the [prime number](prime-number.md) used for that pass. One is excluded throughout.

The saving from starting at $p^2$ is justified by the smaller multiplier: if $p k<p^2$ with $2\leq k<p$, then $k$ has a [prime factor](#prime-factor) $q<p$, so $q$ has already marked $p k$. For $p=7$, the earlier multiples $14,21,28,35,42$ have already been marked using $2,3$ or $5$. The first new possibility is $49$.

For $N=100$, only the [prime numbers](prime-number.md) $2,3,5,7$ need marking passes. They remove all the [composite numbers](number-theory.md#composite-number), leaving **25 [prime numbers](prime-number.md)**. The diagram colors each [composite number](number-theory.md#composite-number) by its smallest [prime factor](#prime-factor), so it shows which marking pass removes it first. The excluded [integer](integer.md) one is shown separately.

<a id="image-the-sieve-of-eratosthenes-leaves-25-prime-numbers-among-the-integers-from-one-to-100"></a>
![](prime-sieve-smallest-factors.png)

**[Figure 2](#image-the-sieve-of-eratosthenes-leaves-25-prime-numbers-among-the-integers-from-one-to-100). The sieve of Eratosthenes leaves 25 prime numbers among the integers from one to 100**. Each colored [composite number](number-theory.md#composite-number) is assigned to its smallest [prime factor](#prime-factor), one of $2,3,5,7$. The green survivors are [prime numbers](prime-number.md); one is neither a [prime number](prime-number.md) nor a [composite number](number-theory.md#composite-number).

Why does the [algorithm](algorithm.md) work? A surviving candidate cannot be a [composite number](number-theory.md#composite-number), since its smaller [prime factor](#prime-factor) would already have removed it. Conversely, marking proper multiples never removes a [prime number](prime-number.md). Every [composite number](number-theory.md#composite-number) at most $N$ has a [prime factor](#prime-factor) at most $\sqrt N$, so no later pass is needed. The [sieve of Eratosthenes](#sieve-of-eratosthenes) is useful when an entire bounded list is wanted; [primality testing](theoretical-computer-science.md#primality-testing) of one large [integer](integer.md) is a different computational task.

The historical name is supported by a surviving primary account: Nicomachus, in Book I, chapter 13 of _Introduction to Arithmetic_, names Eratosthenes and describes separating [prime numbers](prime-number.md) from [composite numbers](number-theory.md#composite-number) by marking multiples among the [odd integers](integer.md#odd-integer) beginning with three. That passage documents the sieve tradition; the bounded [algorithm](algorithm.md) above and its $p^2$ starting rule are the formulation explained here, rather than instructions quoted from [Euclid's Elements](euclidean-geometry.md#euclid-s-elements). [Nicomachus, Introduction to Arithmetic I.13.2–8, Martin Luther D'Ooge translation (1926), revised classroom edition by Nathanael Hahn (2025), pp. 24–25](https://stoicheiamath.com/wp-content/uploads/2025/09/Nicomachus-Introduction-to-Arithmetic-Student-Edition.pdf#page=28)

## Infinitely many primes congruent to one modulo six

↑ **Parent:** [Prime number](prime-number.md)

Assume that $x^2\equiv-3\pmod p$ with $p>3$ implies $p\equiv1\pmod6$. For a finite list of primes in that residue class, let $P$ be their product. Every prime divisor of $4P^2+3$ is greater than three and satisfies that quadratic [modular congruence](modular-arithmetic.md#modular-congruence), hence has residue one modulo six. None is listed because $4P^2+3\equiv3$ modulo a listed prime.

// Target: combinatorics.bigb

## Infinitely many primes congruent to minus one modulo six

↑ **Parent:** [Prime number](prime-number.md)

For any finite list of such [prime numbers](prime-number.md), let $P$ be their product. The integer $6P-1$ has no listed prime divisor, nor the divisors $2,3$. Its remaining prime factors have residues $1,-1$ modulo six, and at least one has residue $-1$ because their product has that residue. Thus no finite list is exhaustive.

// Target: number-theory.bigb

<h2 id="bertrand-s-postulate">Bertrand's postulate</h2>

↑ **Parent:** [Prime number](prime-number.md)

For every integer $n>1$, there is a [prime number](prime-number.md) strictly between $n$ and $2n$. This supplies cyclic prime moduli comparable to an integer interval's length in [additive combinatorics](additive-combinatorics.md).

## Twin prime

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Twin_prime)

Two [primes](prime-number.md) differing by two form a twin-prime pair, for example $3,5$ or $11,13$. The [twin-prime upper bound using Bombieri–Vinogradov](#twin-prime-upper-bound-using-bombieri-vinogradov) limits their number without proving there are infinitely many.

### Twin prime conjecture

↑ **Parent:** [Twin prime](#twin-prime)

The conjecture asserts that infinitely many [prime numbers](prime-number.md) $p$ have $p+2$ prime. The [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture) predicts their quantitative frequency and is stronger. The [Selberg sieve](analytic-number-theory.md#selberg-sieve) supplies an upper bound of the predicted order but does not prove infinitude.

<h4 id="hardy-littlewood-twin-prime-asymptotic-conjecture">Hardy–Littlewood twin-prime asymptotic conjecture</h4>

↑ **Parent:** [Twin prime conjecture](#twin-prime-conjecture)

The local-density prediction for twin primes is the displayed asymptotic, with the [twin-prime constant](#twin-prime-constant) $C_2$. It is stronger than infinitude alone. The [Selberg sieve](analytic-number-theory.md#selberg-sieve) proves the correct order of magnitude as an upper bound, but the [parity problem in sieve theory](analytic-number-theory.md#parity-problem) prevents its elementary majorant from proving this conjectured asymptotic.

// Target: analytic-number-theory.bigb

#### Twin-prime constant

↑ **Parent:** [Twin prime conjecture](#twin-prime-conjecture)

This positive convergent product corrects for the dependence of primality of $n$ and $n+2$ at each odd prime. The associated singular series is $2C_2$: the factor at two is two, and at an odd prime the local correction is $(1-2/p)/(1-1/p)^2$. It appears in the [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture) and in upper bounds from the [Selberg sieve](analytic-number-theory.md#selberg-sieve).

// Target: analytic-number-theory.bigb

<h3 id="brun-s-theorem">Brun's theorem</h3>

↑ **Parent:** [Twin prime](#twin-prime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brun's_theorem)

The sum of reciprocals of [twin primes](#twin-prime) converges, whether or not there are infinitely many [twin primes](#twin-prime). The [twin-prime upper bound from a quadratic sieve](analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve) and [reciprocal-sum convergence from a counting bound](analytic-number-theory.md#reciprocal-sum-convergence-from-a-counting-bound) prove it. This contrasts with the [Euler proof that the sum of reciprocals of primes diverges](analytic-number-theory.md#euler-proof-that-the-sum-of-reciprocals-of-primes-diverges).

<h3 id="twin-prime-upper-bound-using-bombieri-vinogradov">Twin-prime upper bound using Bombieri–Vinogradov</h3>

↑ **Parent:** [Twin prime](#twin-prime)

Apply the [Selberg upper-bound sieve](analytic-number-theory.md#selberg-upper-bound-sieve) to the numbers $p+2$ with $p\leq x$ [prime](prime-number.md). For [odd](calculus.md#odd-function) [squarefree integers](integer.md#square-free-integer) $d$, the local count is $\pi(x;d,-2)$ and the density is $1/\phi(d)$. With sieve level $D=x^{1/3}$, the normalizing sum is $\gg\log x$ by the [truncated Euler-product lower bound](analytic-number-theory.md#truncated-euler-product-lower-bound). The [Selberg least-common-multiple weights](analytic-number-theory.md#selberg-least-common-multiple-weights) have [absolute values](real-analysis.md#absolute-value) at most $3^{\omega(d)}$. The [weighted arithmetic-progression error bound](analytic-number-theory.md#weighted-arithmetic-progression-error-bound) and [Bombieri–Vinogradov theorem](analytic-number-theory.md#bombieri-vinogradov-theorem) make their total error $O(x/\log^3x)$. Consequently the number of [twin prime](#twin-prime) pairs with smaller member at most $x$ is $O(x/\log^2x)$.

<h2 id="euclid-s-theorem">Euclid's theorem</h2>

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid's_theorem)

There are infinitely many [prime numbers](prime-number.md). Indeed, for any finite list of [prime numbers](prime-number.md) $p_1,\ldots,p_k$, the [integer](integer.md) $N=p_1\cdots p_k+1>1$ has a [prime factor](#prime-factor), by the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). None of the listed [prime numbers](prime-number.md) divides $N$, since each divides $N-1$ and a common [divisor](divisibility.md#divisor) would divide $1$. Thus no finite list contains all [prime numbers](prime-number.md). The constructed $N$ need not itself be a [prime number](prime-number.md).

For example, the first six [prime numbers](prime-number.md) give

$$
2\cdot3\cdot5\cdot7\cdot11\cdot13+1=30031=59\cdot509.
$$

Both [prime factors](#prime-factor) lie outside the original list, although $30031$ is a [composite number](number-theory.md#composite-number). The construction defeats a proposed complete list; it is not a formula guaranteed to produce a [prime number](prime-number.md). Book IX, Proposition 20 of [Euclid's Elements](euclidean-geometry.md#euclid-s-elements) explicitly considers both possibilities, prime and composite. [Euclid, Elements, Book IX, Proposition 20: a prime or composite successor](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX20.html).

## Odd prime

↑ **Parent:** [Prime number](prime-number.md)

An odd prime is a [prime number](prime-number.md) that is an [odd integer](integer.md#odd-integer). The only [even number](integer.md#even-number) that is a [prime number](prime-number.md) is $2$, since every other positive [even number](integer.md#even-number) has $2$ as a proper [divisor](divisibility.md#divisor). Thus every [prime number](prime-number.md) greater than $2$ is an odd prime. There are infinitely many odd primes, by [Euclid's theorem](#euclid-s-theorem).

## Fermat prime

↑ **Parent:** [Prime number](prime-number.md)

A [Fermat prime](#fermat-prime) is a [Fermat number](number-theory.md#fermat-number) that is also a [prime number](prime-number.md):

$$
F_k=2^{2^k}+1,\qquad k\geq0.
$$

The defining form alone does not imply [primality](#primality). For example, $65537$ is a [Fermat prime](#fermat-prime), while $4294967297$ is a [Fermat number](number-theory.md#fermat-number) with proper [divisors](divisibility.md#divisor). For $k\geq1$, every [Fermat prime](#fermat-prime) is one modulo four and two modulo three. [Pépin's test](#pepin-s-test) gives an exact [primality testing](theoretical-computer-science.md#primality-testing) criterion for these candidates, rather than relying on their form.

<h3 id="pepin-s-test">Pépin's test</h3>

↑ **Parent:** [Fermat prime](#fermat-prime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pépin's_test)

For $n\geq1$, [Pépin's test](#pepin-s-test) says that the [Fermat number](number-theory.md#fermat-number) $F_n$ is a [prime number](prime-number.md) exactly when the displayed [modular congruence](modular-arithmetic.md#modular-congruence) holds. [Modular exponentiation](number-theory.md#modular-exponentiation) evaluates it by [exponentiation by squaring](number-theory.md#exponentiation-by-squaring) without constructing the enormous ordinary power. The index restriction excludes $F_0=3$, where the base itself is divisible by the candidate.[slide 14](mathematics-bibliography.md#primality-testing-then-and-now-by-carl-pomerance)

For a proof outline of sufficiency, any [prime factor](#prime-factor) $p$ of a passing candidate gives $3$ [multiplicative order](number-theory.md#multiplicative-order) exactly $F_n-1$, a [power of two](integer.md#power-of-two): its half-power is $-1$, rather than $1$. [Fermat's little theorem](number-theory.md#fermat-little-theorem) forces $F_n-1\mid p-1$, so $p\geq F_n$, and hence $p=F_n$. Conversely, for a prime candidate, $F_n\equiv5\pmod{12}$; [quadratic reciprocity](number-theory.md#quadratic-reciprocity) and [Euler's criterion](quadratic-residue.md#euler-s-criterion) give the required half-power. At $n=1$, the check is $3^2\equiv4=-1\pmod5$.

### Quadratic nonresidues modulo a Fermat prime

↑ **Parent:** [Fermat prime](#fermat-prime)

For a Fermat prime $p=2^{2^k}+1$, the multiplicative group modulo $p$ has order $2^{2^k}$. Its $\varphi(p-1)=(p-1)/2$ primitive roots are all quadratic nonresidues; since there are also $(p-1)/2$ nonresidues, the two sets coincide.

## Fundamental theorem of arithmetic

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic)

Every [integer](integer.md) $n>1$ is a [product](arithmetic.md#product-of-numbers) of [prime numbers](prime-number.md), uniquely up to reordering the factors. More precisely, there are unique distinct [prime numbers](prime-number.md) $p_1<\cdots<p_r$ and unique positive [integer](integer.md) exponents $a_1,\ldots,a_r$ such that

$$
n=p_1^{a_1}\cdots p_r^{a_r}.
$$

In the header's displayed form, $v_p(n)$ is the [prime valuation](number-theory.md#prime-valuation), the exponent of $p$ in this [prime factorization](#fundamental-theorem-of-arithmetic); it is zero when $p$ does not divide $n$. Reordering or regrouping the [prime factors](#prime-factor) does not give a different [prime factorization](#fundamental-theorem-of-arithmetic).

For $360$, repeated [division](arithmetic.md#division-mathematics) gives $360/2=180$, $180/2=90$, $90/2=45$, then $45/3=15$, $15/3=5$, and $5/5=1$. Thus

$$
360=2\cdot2\cdot2\cdot3\cdot3\cdot5=2^3\cdot3^2\cdot5,
\qquad 2^3\cdot3^2\cdot5=8\cdot9\cdot5=360.
$$

Its nonzero [prime valuations](number-theory.md#prime-valuation) are $v_2(360)=3$, $v_3(360)=2$ and $v_5(360)=1$. Recording only the distinct [prime factors](#prime-factor) $2,3,5$ would lose the difference between $30$ and $360$.

This turns [divisibility](divisibility.md) into coordinatewise comparison of nonnegative exponents. A positive [divisor](divisibility.md#divisor) of $360$ chooses an exponent from $0,1,2,3$ for $2$, from $0,1,2$ for $3$, and from $0,1$ for $5$, giving $4\cdot3\cdot2=24$ positive [divisors](divisibility.md#divisor). The [greatest common divisor](divisibility.md#greatest-common-divisor) takes the smaller exponent at each [prime number](prime-number.md); the [least common multiple](divisibility.md#least-common-multiple) takes the larger. The theorem is a structural description, not an assertion that finding the factors of every large [integer](integer.md) is computationally easy.

In general, for [positive integers](integer.md#positive-integer) $d,n$, the exact [divisibility](divisibility.md) criterion is

$$
d\mid n\quad\Longleftrightarrow\quad v_p(d)\leq v_p(n)\ \text{for every prime }p.
$$

For example, $72=2^3\cdot3^2$ divides $360$, with quotient $5$, whereas $48=2^4\cdot3$ does not: it requires four factors of two, but $360$ supplies only three. Both use only [prime factors](#prime-factor) of $360$, so membership in that list alone does not establish [divisibility](divisibility.md). Every positive [divisor](divisibility.md#divisor) of $360$ is uniquely $2^a3^b5^c$ with $0\leq a\leq3$, $0\leq b\leq2$, $0\leq c\leq1$. Sorted, all 24 positive [divisors](divisibility.md#divisor) are

$$
\begin{gathered}
1,2,3,4,5,6,8,9,10,12,15,18,\\
20,24,30,36,40,45,60,72,90,120,180,360.
\end{gathered}
$$

Thus the [divisor function](arithmetic-function.md#divisor-function) gives $\tau(360)=(3+1)(2+1)(1+1)=24$. These include [divisors](divisibility.md#divisor) that are [composite numbers](number-theory.md#composite-number), as well as the [prime factors](#prime-factor) and one.

For another [positive integer](integer.md#positive-integer) $m$, the [prime valuations](number-theory.md#prime-valuation) give exact formulas for the [greatest common divisor](divisibility.md#greatest-common-divisor) and [least common multiple](divisibility.md#least-common-multiple):

$$
\begin{aligned}
v_p(\gcd(n,m))&=\min\{v_p(n),v_p(m)\},\\
v_p(\operatorname{lcm}(n,m))&=\max\{v_p(n),v_p(m)\}.
\end{aligned}
$$

With $n=360$ and $m=84=2^2\cdot3\cdot7$, their [prime valuations](number-theory.md#prime-valuation) at $2,3,5,7$ are $(3,2,1,0)$ and $(2,1,0,1)$. The smaller exponents give $(2,1,0,0)$, and the larger give $(3,2,1,1)$, hence

$$
\gcd(360,84)=2^2\cdot3=12,\qquad
\operatorname{lcm}(360,84)=2^3\cdot3^2\cdot5\cdot7=2520.
$$

Indeed, $360/12=30$, $84/12=7$, $2520/360=7$ and $2520/84=30$. The same rules also explain $\gcd(n,m)\operatorname{lcm}(n,m)=nm$: the smaller and larger exponents sum to the two original exponents. Here $12\cdot2520=360\cdot84=30240$.

<a id="image-prime-valuations-compute-the-greatest-common-divisor-least-common-multiple-and-all-24-positive-divisors-of-360"></a>
![](prime-factorization-exponents.png)

**[Figure 3](#image-prime-valuations-compute-the-greatest-common-divisor-least-common-multiple-and-all-24-positive-divisors-of-360). Prime valuations compute the greatest common divisor, least common multiple and all 24 positive divisors of 360**. The upper table compares exponents at the [prime numbers](prime-number.md) $2,3,5,7$ for $360$ and $84$, then takes their columnwise minimum and maximum. The lower tables enumerate $2^a3^b5^c$ for $c=0$ and $c=1$; each cell gives one positive [divisor](divisibility.md#divisor).

The useful change of viewpoint is that [multiplication](arithmetic.md#multiplication) becomes [addition](arithmetic.md#addition) of [prime valuations](number-theory.md#prime-valuation), $v_p(nm)=v_p(n)+v_p(m)$, and [divisibility](divisibility.md) becomes comparison. Many different-looking calculations therefore share one representation. The [prime valuations](number-theory.md#prime-valuation) are coordinates for [multiplication](arithmetic.md#multiplication), rather than digits in [positional notation](integer.md#positional-notation): they do not turn ordinary [addition](arithmetic.md#addition) of [integers](integer.md) into coordinatewise [addition](arithmetic.md#addition).

Different intermediate splits lead to the same prime ingredients. Starting with $360=36\cdot10$ gives $36=6\cdot6$ and $10=2\cdot5$; starting with $360=8\cdot45$ gives $8=2\cdot4$ and $45=5\cdot9$. Continuing to split the [composite numbers](number-theory.md#composite-number) produces the same [multiset](set.md#multiset) of [prime factors](#prime-factor): three twos, two threes, and one five. The [factorization tree](#factorization-tree) records choices in the calculation, while the [prime factorization](#fundamental-theorem-of-arithmetic) records the invariant result.

<a id="image-two-factorization-trees-for-360-give-the-same-prime-factorization-2-3-cdot3-2-cdot5"></a>
![](prime-factorization-trees.png)

**[Figure 4](#image-two-factorization-trees-for-360-give-the-same-prime-factorization-2-3-cdot3-2-cdot5). Two factorization trees for $360$ give the same prime factorization $2^3\cdot3^2\cdot5$**.

The proof outline explains the uniqueness. Existence follows by splitting a [composite number](number-theory.md#composite-number) into smaller factors until only [prime numbers](prime-number.md) remain. For uniqueness, [Euclid's lemma](number-theory.md#euclid-s-lemma) says that a [prime factor](#prime-factor) of one [product](arithmetic.md#product-of-numbers) must divide one factor of any other prime [product](arithmetic.md#product-of-numbers) equal to it. That factor must be the same [prime number](prime-number.md); cancel it and repeat. The crucial [divisibility](divisibility.md) step appears in Book VII, Proposition 30 of [Euclid's Elements](euclidean-geometry.md#euclid-s-elements). [Euclid, Elements VII.30: a prime divisor of a product](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII30.html)

The ancient text supplies specific precursors to the modern statement: Book VII, Proposition 31 establishes that every [composite number](number-theory.md#composite-number) has a [prime factor](#prime-factor), and Book IX, Proposition 14 excludes any new [prime factor](#prime-factor) from the [least common multiple](divisibility.md#least-common-multiple) of given [prime numbers](prime-number.md). These are the propositions being cited, rather than the complete modern exponent formulation of the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). [Euclid, Elements VII.31: every composite number has a prime divisor](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII31.html) [Euclid, Elements IX.14: prime divisors of a least common multiple of primes](https://mathcs.clarku.edu/~djoyce/java/elements/bookIX/propIX14.html)

Excluding one from the [prime numbers](prime-number.md) keeps uniqueness meaningful: otherwise $360=2^3\cdot3^2\cdot5=1\cdot2^3\cdot3^2\cdot5=1\cdot1\cdot2^3\cdot3^2\cdot5$ would give different collections of supposed [prime factors](#prime-factor). For $n=1$, the natural convention is the [empty product](arithmetic.md#empty-product), equal to one, with no [prime factors](#prime-factor) and all [prime valuations](number-theory.md#prime-valuation) zero.

### Prime signature

↑ **Parent:** [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)

The prime signature of $n=\prod_{i=1}^r p_i^{a_i}$ is the [multiset](set.md#multiset) of positive [prime exponents](number-theory.md#p-adic-valuation) $a_i$, conventionally sorted. For example, $12=2^2\cdot3$ and $45=3^2\cdot5$ both have signature $(2,1)$. Quantities such as the [divisor function](arithmetic-function.md#divisor-function) and the number of [ordered factorizations](number-theory.md#ordered-factorization) depend on this signature rather than the particular [primes](prime-number.md).

### Factorization tree

↑ **Parent:** [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)

A [factorization tree](#factorization-tree) is a [rooted tree](tree-graph-theory.md#rooted-tree) whose root is an [integer](integer.md) $n>1$. Each nonleaf label is a [composite number](number-theory.md#composite-number) split into two factors greater than one whose [product](arithmetic.md#product-of-numbers) equals that label; the leaves are [prime numbers](prime-number.md). Multiplying the leaves recovers $n$. Many [factorization trees](#factorization-tree) can have the same root, but the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic) gives them the same leaf [multiset](set.md#multiset).

## Prime factor

↑ **Parent:** [Prime number](prime-number.md)

A [prime factor](#prime-factor) of a nonzero [integer](integer.md) $n$ is a [prime number](prime-number.md) $p$ satisfying $p\mid n$. For $360=2^3\cdot3^2\cdot5$, the distinct [prime factors](#prime-factor) are $2,3,5$, while counting repeated factors gives six prime entries. A [prime factorization](#fundamental-theorem-of-arithmetic) retains their multiplicities: knowing only the distinct [prime factors](#prime-factor) does not distinguish $12=2^2\cdot3$ from $18=2\cdot3^2$. A negative [integer](integer.md) has the same [prime factors](#prime-factor) as its [absolute value](real-analysis.md#absolute-value).

### Smallest prime factor

↑ **Parent:** [Prime factor](#prime-factor)

## Prime power

↑ **Parent:** [Prime number](prime-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_power)

A prime power is a positive integer of the form $p^d$, where $p$ is a [prime number](prime-number.md) and $d$ is a nonnegative integer.

## ↑ Ancestors (4)

1. [Number theory](number-theory.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (262)

- [2-adic absolute value](non-archimedean-analysis.md#2-adic-absolute-value)
- [2-adic valuation](number-theory.md#2-adic-valuation)
- [A group of prime order is cyclic](group.md#a-group-of-prime-order-is-cyclic)
- [Additive category with truncated primary torsion](category-theory.md#additive-category-with-truncated-primary-torsion)
- [Affine Galois group of a prime-radical splitting field](group-theory.md#affine-galois-group-of-a-prime-radical-splitting-field)
- [Algebraic number theory](algebraic-number-theory.md)
- [Analytic number theory](analytic-number-theory.md)
- [Base-p digit sum](number-theory.md#base-p-digit-sum)
- [Bertrand's postulate](#bertrand-s-postulate)
- [Carmichael function](number-theory.md#carmichael-function)
- [Carmichael number](number-theory.md#carmichael-number)
- [Character degree coprime to p from the core tower](representation-theory-of-the-symmetric-group.md#character-degree-coprime-to-p-from-the-core-tower)
- [Chebyshev function](arithmetic-function.md#chebyshev-function)
- [Chebyshev theta function](number-theory.md#chebyshev-theta-function)
- [Circular prime](#circular-prime)
- [Complementary factorial congruence](modular-arithmetic.md#complementary-factorial-congruence)
- [Completely multiplicative function](arithmetic-function.md#completely-multiplicative-function)
- [Composite number](number-theory.md#composite-number)
- [Congruence of squares](number-theory.md#congruence-of-squares)
- [Congruence submonoid of the positive integers](algebraic-operation.md#congruence-submonoid-of-the-positive-integers)
- [Coprime integers](divisibility.md#coprime-integers)
- [Counting cycles in an interval covering graph](discrete-dynamical-system.md#counting-cycles-in-an-interval-covering-graph)
- [Cramér model](analytic-number-theory.md#cramer-model)
- [Cuban prime](#cuban-prime)
- [Decisive number](number-theory.md#decisive-number)
- [Divisor](divisibility.md#divisor)
- [Divisor function](arithmetic-function.md#divisor-function)
- [ElGamal signature scheme](computer-science.md#elgamal-signature-scheme)
- [Euclid-Euler theorem](integer.md#euclid-euler-theorem)
- [Euclid's lemma](number-theory.md#euclid-s-lemma)
- [Euclid's theorem](#euclid-s-theorem)
- [Euler product](analytic-number-theory.md#euler-product)
- [Euler's criterion](quadratic-residue.md#euler-s-criterion)
- [Euler's theorem](number-theory.md#euler-s-theorem)
- [Factor base](number-theory.md#factor-base)
- [Factorization tree](#factorization-tree)
- [Fermat little theorem](number-theory.md#fermat-little-theorem)
- [Fermat number](number-theory.md#fermat-number)
- [Fermat prime](#fermat-prime)
- [Fermat test example](number-theory.md#fermat-test-example)
- [Field](algebra.md#field)
- [Finite field](algebra.md#finite-field)
- [Finite p-group](finite-group-theory.md#finite-p-group)
- [Finite separating-functional proof of the columns condition](ramsey-theory.md#finite-separating-functional-proof-of-the-columns-condition)
- [Finite simple group](finite-group-theory.md#finite-simple-group)
- [Frankl-Wilson theorem](extremal-set-theory.md#frankl-wilson-theorem)
- [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)
- [Greatest common divisor](divisibility.md#greatest-common-divisor)
- [Identity for Dirichlet convolution](arithmetic-function.md#identity-for-dirichlet-convolution)
- [Infinite field of positive characteristic from an ultraproduct](model-theory.md#infinite-field-of-positive-characteristic-from-an-ultraproduct)
- [Infinitely many primes congruent to minus one modulo six](#infinitely-many-primes-congruent-to-minus-one-modulo-six)
- [Integer factorization](number-theory.md#integer-factorization)
- [Integer localization at a set of primes](commutative-algebra.md#integer-localization-at-a-set-of-primes)
- [Irreducibility of cyclotomic polynomials](galois-theory.md#irreducibility-of-cyclotomic-polynomials)
- [Irreducible characters of degree coprime to p](representation-theory.md#irreducible-characters-of-degree-coprime-to-p)
- [Irreducible element of a commutative monoid](algebraic-operation.md#irreducible-element-of-a-commutative-monoid)
- [Korselt criterion](number-theory.md#korselt-criterion)
- [Kummer's theorem](number-theory.md#kummer-s-theorem)
- [Largest prime factor](number-theory.md#largest-prime-factor)
- [Last nonzero digit coloring](ramsey-theory.md#last-nonzero-digit-coloring)
- [Leading-residue obstruction to partition regularity](ramsey-theory.md#leading-residue-obstruction-to-partition-regularity)
- [Least common multiple](divisibility.md#least-common-multiple)
- [Legendre's formula](number-theory.md#legendre-s-formula)
- [Linear sieve](algorithm.md#linear-sieve)
- [Lucas's theorem](binomial-coefficient.md#lucas-s-theorem)
- [Mathematical proof](foundations-of-mathematics.md#mathematical-proof)
- [Mersenne prime](integer.md#mersenne-prime)
- [Minimal cyclic factorization criterion for powerful p-groups](finite-group-theory.md#minimal-cyclic-factorization-criterion-for-powerful-p-groups)
- [Möbius function](arithmetic-function.md#mobius-function)
- [Möbius inversion formula](arithmetic-function.md#mobius-inversion-formula)
- [Modular intersection graph](extremal-set-theory.md#modular-intersection-graph)
- [Modular intersection polynomial](extremal-set-theory.md#modular-intersection-polynomial)
- [Modular layer vanishing lemma](extremal-set-theory.md#modular-layer-vanishing-lemma)
- [Modular-size auxiliary polynomials](extremal-set-theory.md#modular-size-auxiliary-polynomials)
- [Monoid automorphism](algebraic-operation.md#monoid-automorphism)
- [Multiplicative function](arithmetic-function.md#multiplicative-function)
- [Multiplicativity of the Legendre symbol](quadratic-residue.md#multiplicativity-of-the-legendre-symbol)
- [Natural density](number-theory.md#natural-density)
- [Non-Archimedean place of a number field](algebraic-number-theory.md#non-archimedean-place-of-a-number-field)
- [Nonabelian group of order pq](finite-group-theory.md#nonabelian-group-of-order-pq)
- [Nontrivial square root of unity modulo an integer](number-theory.md#nontrivial-square-root-of-unity-modulo-an-integer)
- [Nonuniform Frankl-Wilson theorem](extremal-set-theory.md#nonuniform-frankl-wilson-theorem)
- [Nonzero residue permutation](number-theory.md#nonzero-residue-permutation)
- [Number-theoretic sieve](algorithm.md#number-theoretic-sieve)
- [Number theory](number-theory.md)
- [Odd prime](#odd-prime)
- [p-adic absolute value](non-archimedean-analysis.md#p-adic-absolute-value)
- [p-adic integer](number-theory.md#p-adic-integer)
- [P-adic number](non-archimedean-analysis.md#p-adic-number)
- [P-adic valuation](number-theory.md#p-adic-valuation)
- [P-deficiency](geometric-group-theory.md#p-deficiency)
- [p-valuation](associative-algebra.md#p-valuation)
- [Pandigital prime](integer.md#pandigital-prime)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#5e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#6e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#7e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-10.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4.md#6c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#6e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-12.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#11c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#2c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4.md#7e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5.md#12/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-12.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4.md#7d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#2g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-27.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#1e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#6e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#12h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#1g/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-9.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#1i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#11i/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#1i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#1i/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-10.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-10.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#2d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#6d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3.md#6d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#6e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#6e/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4.md#5e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4.md#6e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#5d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#5d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#5d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#11h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#10g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#3g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-130.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2.md#11g/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3.md#11g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#20g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-130.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-3.md#5d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#11i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#18f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-150.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#11h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#1h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#11h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4.md#6e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#1i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-130.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-160.md#2/d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3.md#5e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4.md#5e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#20h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-120.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4.md#9e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#1g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#1g/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101.md#1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-130.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-133.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-137.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-160.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-109.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-130.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-130.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166.md#2/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-150.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-166.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#8/solution)
- [Pépin's test](#pepin-s-test)
- [Power-core truncation of a prime-core tower](representation-theory-of-the-symmetric-group.md#power-core-truncation-of-a-prime-core-tower)
- [Primality](#primality)
- [Primality testing](theoretical-computer-science.md#primality-testing)
- [Prime coefficient detection of quasi-isomorphisms](homology.md#prime-coefficient-detection-of-quasi-isomorphisms)
- [Prime counting](number-theory.md#prime-counting)
- [Prime-divisibility coding of a finite set](mathematical-logic.md#prime-divisibility-coding-of-a-finite-set)
- [Prime divisor of a Fermat number](number-theory.md#prime-divisor-of-a-fermat-number)
- [Prime-exponent encoding of a finite list](mathematical-logic.md#prime-exponent-encoding-of-a-finite-list)
- [Prime factor](#prime-factor)
- [Prime field](algebra.md#prime-field)
- [Prime number](prime-number.md)
- [Prime omega function](arithmetic-function.md#prime-omega-function)
- [Prime power](#prime-power)
- [Prime-power binomial divisibility](binomial-coefficient.md#prime-power-binomial-divisibility)
- [Prime-power coefficients of a level-one eigenform are often large and positive](modular-function.md#prime-power-coefficients-of-a-level-one-eigenform-are-often-large-and-positive)
- [Prime-proof number](theoretical-computer-science.md#prime-proof-number)
- [Prime-row binomial coefficient divisibility](binomial-coefficient.md#prime-row-binomial-coefficient-divisibility)
- [Prime sieve](algorithm.md#prime-sieve)
- [Prime sum](analytic-number-theory.md#prime-sum)
- [Prime valuation](number-theory.md#prime-valuation)
- [Prime-valued sum](arithmetic.md#prime-valued-sum)
- [Quadratic reciprocity](number-theory.md#quadratic-reciprocity)
- [Quadratic residue](quadratic-residue.md)
- [Radical of an integer](arithmetic-function.md#radical-of-an-integer)
- [Reduction modulo a prime in an integral matrix group](group-theory.md#reduction-modulo-a-prime-in-an-integral-matrix-group)
- [Repdigit](integer.md#repdigit)
- [Ridout theorem](diophantine-approximation.md#ridout-theorem)
- [Ring of integers of Q of pth root p](algebraic-number-theory.md#ring-of-integers-of-q-of-pth-root-p)
- [S-smooth number](number-theory.md#s-smooth-number)
- [Second Chebyshev function](arithmetic-function.md#second-chebyshev-function)
- [Semiprime](number-theory.md#semiprime)
- [Sieve of Eratosthenes](#sieve-of-eratosthenes)
- [Square-free integer](integer.md#square-free-integer)
- [Squarefree-part bound for smooth numbers](number-theory.md#squarefree-part-bound-for-smooth-numbers)
- [Sqube](integer.md#sqube)
- [Strong induction for factorization existence](foundations-of-mathematics.md#strong-induction-for-factorization-existence)
- [Strong-pseudoprime bases for a product of two primes with common predecessor divisor ten](number-theory.md#strong-pseudoprime-bases-for-a-product-of-two-primes-with-common-predecessor-divisor-ten)
- [Subadditivity of the base-p digit sum](number-theory.md#subadditivity-of-the-base-p-digit-sum)
- [Sum-of-divisors function](arithmetic-function.md#sum-of-divisors-function)
- [Summatory function](arithmetic-function.md#summatory-function)
- [Tate module](representation-theory.md#tate-module)
- [Total number of prime factors](arithmetic-function.md#total-number-of-prime-factors)
- [Trial division](#trial-division)
- [Truncatable prime](#truncatable-prime)
- [Twin prime conjecture](#twin-prime-conjecture)
- [Two distinguished classes of discriminant minus eight q](number-theory.md#two-distinguished-classes-of-discriminant-minus-eight-q)
- [Unit modulo n](modular-arithmetic.md#unit-modulo-n)
- [Upper asymptotic density](number-theory.md#upper-asymptotic-density)
- [Von Mangoldt divisor identity](arithmetic-function.md#von-mangoldt-divisor-identity)
- [Von Mangoldt function](arithmetic-function.md#von-mangoldt-function)
- [Wilson factorial congruence modulo a triangular number](modular-arithmetic.md#wilson-factorial-congruence-modulo-a-triangular-number)
- [Wilson's theorem](modular-arithmetic.md#wilson-s-theorem)
