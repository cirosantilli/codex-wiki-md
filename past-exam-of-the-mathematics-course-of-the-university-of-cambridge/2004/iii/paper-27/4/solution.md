<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [cyclotomic Euler system](../../../../../cyclotomic-euler-system.md) must relate [units](../../../../../unit-in-a-ring.md) at many auxiliary conductors, not just the successive layers of one p-power tower. A useful axiomatization is the [root-of-unity Euler system](../../../../../root-of-unity-euler-system.md). Fix a finite set of excluded primes $S$ containing $2$, and let $W_S$ be the [roots of unity](../../../../../root-of-unity.md) whose orders are prime to every prime in $S$. A system is a nonzero-valued function $\Phi:W_S\to\overline{\mathbb Q}^{\times}$ with three properties. It is even and Galois equivariant:

$$
\Phi(\xi^{-1})=\Phi(\xi),\qquad \Phi(\xi^\sigma)=\Phi(\xi)^\sigma.
$$

It satisfies the distribution relation at every prime $\ell\notin S$:

$$
\prod_{\rho\in\mu_\ell}\Phi(\rho\xi)=\Phi(\xi^\ell).
$$

Finally, if $\ell\nmid\operatorname{ord}(\xi)$, it satisfies the local congruence

$$
\Phi(\rho\xi)\equiv\Phi(\xi)\pmod{\mathfrak l}
\qquad(\rho\in\mu_\ell,\ \mathfrak l\mid\ell).
$$

The values in this congruence are required to be integral at the prime; in the [unit](../../../../../unit-in-a-ring.md) example below they are local [units](../../../../../unit-in-a-ring.md). Evenness puts the values in the maximal real cyclotomic subfields. Equivariance identifies conjugates, distribution gives exact norm identities, and the congruence supplies information at newly introduced primes. These are the three distinct inputs used in the descent, rather than a single norm-coherence assumption.

Here is a concrete system extending the [units](../../../../../unit-in-a-ring.md) in Q2. Fix a nonzero integer $a$ prime to $p$ and let $S$ contain $2$ and the prime divisors of $a$, but not $p$. Put

$$
\Phi_a(\xi)=\left(\frac{\xi^{-a}-\xi^a}{\xi^{-1}-\xi}\right)^{p-1}\quad(\xi\ne1),
\qquad\Phi_a(1)=a^{p-1}.
$$

Every value is defined and nonzero: the excluded primes make $a$ invertible modulo the order of $\xi$, and that order is odd. The quotient is the same [Laurent polynomial](../../../../../laurent-polynomial.md) $b_a$ used in Q2. Replacing $\xi$ by $\xi^{-1}$ changes both numerator and denominator by a minus sign, so it is even; its rational coefficients give Galois equivariance.

For the distribution axiom, $\ell\notin S$ makes $\ell$ odd and prime to $a$. Both exponents $2$ and $2a$ permute $\mu_\ell$, and $\prod_{\rho\in\mu_\ell}\rho=1$. The calculation in Q2 therefore holds with $p$ replaced by $\ell$:

$$
\prod_{\rho\in\mu_\ell}b_a(\rho X)=b_a(X^\ell).
$$

Raising to $p-1$ proves the axiom. At removable points it holds by evaluating the regular Laurent polynomials, so it includes $\xi=1$ and $\xi^\ell=1$.

For the congruence axiom, a root $\rho$ of order $\ell$ reduces to one at every prime above $\ell$. The integral [Laurent polynomial](../../../../../laurent-polynomial.md) $b_a$ thus gives $b_a(\rho\xi)\equiv b_a(\xi)$. These values are local [units](../../../../../unit-in-a-ring.md) when $\xi$ has order prime to $\ell$: its reduction retains that order, and, unless $\xi=1$, both $1-\xi^2$ and $1-\xi^{2a}$ remain nonzero; at $\xi=1$ the value is the [unit](../../../../../unit-in-a-ring.md) $a$. The stated power preserves the congruence. Thus **$\Phi_a$ satisfies all three Euler-system axioms**, and its values at $\zeta_n$ are precisely $c_n(a)$. Products, Galois translates, suitable [field norms](../../../../../field-norm.md) and integral group-ring powers produce the other cyclotomic-unit systems needed in the theory.

The distribution relation explains the Euler factors. If $\ell\nmid m$, $\xi$ has order $m$ and $\rho$ is a primitive $\ell$th root, the conjugates over $\mathbb Q(\mu_m)$ run through the nontrivial $\ell$th roots. Removing the single factor with $\rho=1$ from the distribution product gives

$$
N_{\mathbb Q(\mu_{m\ell})/\mathbb Q(\mu_m)}\Phi(\rho\xi)
=\frac{\Phi(\xi^\ell)}{\Phi(\xi)}
=\Phi(\xi)^{\operatorname{Fr}_\ell-1}.
$$

We use arithmetic [Frobenius](../../../../../frobenius-automorphism.md), so $\operatorname{Fr}_\ell(\xi)=\xi^\ell$. This is the [cyclotomic Euler norm factor at a new prime](../../../../../cyclotomic-euler-norm-factor-at-a-new-prime.md). At a higher power of a prime already dividing the conductor, all $\ell$ translates occur, and the ordinary successive-layer norm relation has no missing-factor quotient. A mere p-power compatible sequence therefore contains only part of the Euler-system information.

To explain the axiomatic method, fix a p-power modulus $P=p^r$ and auxiliary primes $\ell$ with $P\mid\ell-1$, split in the chosen real base [field](../../../../../field.md). For the cyclic auxiliary [Galois group](../../../../../galois-group.md) of order $\ell-1$, choose a generator $\sigma_\ell$ and define

$$
D_\ell=\sum_{i=1}^{\ell-2}i\sigma_\ell^i,
\qquad N_\ell=\sum_{i=0}^{\ell-2}\sigma_\ell^i.
$$

Subtracting consecutive coefficients gives the concrete identity

$$
\boxed{(\sigma_\ell-1)D_\ell=(\ell-1)-N_\ell\equiv-N_\ell\pmod P.}
$$

This is the [Kolyvagin derivative operator for a cyclic group](../../../../../kolyvagin-derivative-operator-for-a-cyclic-group.md). Apply products of these operators to Euler-system values at squarefree auxiliary conductors. The norm relations control the apparent failure of invariance modulo $P$; Kummer descent, using [Hilbert 90](../../../../../hilbert-s-theorem-90.md) and retaining roots-of-unity corrections where present, turns the derivative data into classes over the base [field](../../../../../field.md). They have controlled valuations and are unramified away from the selected auxiliary primes and the excluded set. The local congruence relates the valuation component at a newly added prime to the finite residue-symbol component of the preceding class, with the sign and normalization determined by the chosen generator. This finite-to-singular relation is precisely the additional information not obtainable from norm compatibility alone.

The [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md) supplies auxiliary prime ideals in specified ideal classes while satisfying the splitting and congruence conditions. Reading the controlled valuations as principal-ideal relations successively bounds the p-primary elementary divisors of the [ideal class group](../../../../../ideal-class-group.md) by the divisibility of the initial cyclotomic-unit class. On suitable nontrivial character components this gives the finite bound $\#A^\chi\leq\#(E/C)^\chi$; passing through the norm tower yields

$$
\boxed{\operatorname{char}(Y)\mid\operatorname{char}(\mathcal E/\mathcal C),}
$$

where divisibility is between characteristic generators, so the associated ideal containment is reversed. The [Euler-system divisibility for real cyclotomic class modules](../../../../../euler-system-divisibility-for-real-cyclotomic-class-modules.md) requires the usual local conditions and control of finite errors; it is not a claim that arbitrary compatible [units](../../../../../unit-in-a-ring.md) automatically annihilate every class group. The [cyclotomic unit index formula](../../../../../cyclotomic-unit-index-formula.md), together with the global norm-defect comparison, gives the reverse equality. Q3's [exact sequence](../../../../../exact-sequence.md) then proves the main conjecture.

This account separates the theorem inputs from the explicit calculations: the distribution and congruence identities for [cyclotomic units](../../../../../cyclotomic-unit.md) are verified above, and the derivative operator is computed directly; the Chebotarev/Kummer descent bounds and the global index comparison are the deeper arithmetic steps. Their usefulness is that the descent uses the axioms rather than a special closed formula for each individual auxiliary [unit](../../../../../unit-in-a-ring.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
