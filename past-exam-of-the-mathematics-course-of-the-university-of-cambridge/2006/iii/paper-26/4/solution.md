<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $F_n=K_n^+$, $F_\infty=\bigcup_nF_n$, $G=\operatorname{Gal}(F_\infty/\mathbb Q)=\Delta^+\times\Gamma$, where $|\Delta^+|=(p-1)/2$ and $\Gamma\simeq\mathbb Z_p$. Set $A=\mathbb Z_p[[G]]$. Choosing a topological generator $\gamma$ of $\Gamma$ identifies its [Iwasawa algebra](../../../../../iwasawa-algebra.md) with $\Lambda=\mathbb Z_p[[S]]$, $S=\gamma-1$; this group variable is distinct from the local-unit interpolation variable $T$. The [Teichmüller character](../../../../../teichmuller-character.md) decomposes $A$ into a product of copies of $\Lambda$, one for each character of $\Delta^+$, equivalently each even Teichmüller character of $\operatorname{Gal}(K_0/\mathbb Q)$. All characteristic-ideal statements below are componentwise in this product.

Let $U_n^1$ be the local [principal units](../../../../../principal-unit.md) at the unique prime above $p$. Let $E_n^1$ and $C_n^1$ be respectively the p-adic closures of [global units](../../../../../global-unit-of-a-number-field.md) and [cyclotomic units](../../../../../cyclotomic-unit.md) inside $U_n^1$, and take their [inverse limits](../../../../../inverse-limit.md) under the [field norms](../../../../../field-norm.md). Define $X_\infty$ as the [Galois group](../../../../../galois-group.md) of the maximal abelian pro-p extension of $F_\infty$ unramified away from $p$, and $Y_\infty$ as that of the maximal everywhere unramified extension. This is the real tower: its prime-ramified module is torsion, by the [Leopoldt theorem for abelian number fields](../../../../../leopoldt-theorem-for-abelian-number-fields.md). It must not be confused with the positive-rank prime-ramified module of the full complex cyclotomic tower. The [unramified Iwasawa torsion theorem](../../../../../unramified-iwasawa-torsion-theorem.md) gives torsion for $Y_\infty$.

A convenient formulation of the [Iwasawa main conjecture](../../../../../main-conjecture-of-iwasawa-theory.md) uses the [p-adic zeta pseudomeasure](../../../../../p-adic-zeta-pseudomeasure.md) $\zeta_p$ on $G$. With the sign convention

$$
\int x^k\,d\zeta_p=(1-p^{k-1})\zeta(1-k)
=-(1-p^{k-1})\frac{B_k}{k}\qquad(k\ge2\text{ even}),
$$

its product with the [augmentation ideal](../../../../../augmentation-ideal.md) $I(G)$ is integral and principal. The pole on the trivial-character component is cancelled by that ideal; simply writing an integral quotient by $\zeta_p$ would be incorrect. The main assertion in this convention is

$$
\boxed{\operatorname{char}_A(X_\infty)=I(G)\zeta_p.}
$$

We explain the local calculation, the remaining global obstruction, and how the [cyclotomic Euler system](../../../../../cyclotomic-euler-system.md) removes it.

The local calculation is the [Iwasawa theorem on local cyclotomic units](../../../../../iwasawa-theorem-on-local-cyclotomic-units.md):

$$
U_\infty^1/C_\infty^1\simeq A/(I(G)\zeta_p).
$$

One can see why this theorem has exactly this analytic term. For a norm-fixed [Coleman power series](../../../../../coleman-power-series.md) $f$, its corrected logarithm is

$$
\mathcal L(f)=\frac1p\log\frac{f(T)^p}{f((1+T)^p-1)}.
$$

The ratio lies in $1+pR$, so the expression is integral. The norm identity puts its [Amice transform](../../../../../amice-transform.md) in the kernel of the [Coleman trace operator](../../../../../coleman-trace-operator.md), hence gives a measure on $\mathbb Z_p^\times$. Its kth moment is $(1-p^{k-1})\delta_k(f)$. The full local [exact sequence](../../../../../exact-sequence.md) has p-power [roots of unity](../../../../../root-of-unity.md) at its kernel and cokernel. Passing to the real, or even, part removes both, since complex conjugation acts as minus one on their Tate module and $p$ is odd. The corrected logarithm therefore identifies $U_\infty^1$ with $A$.

Question 2 now shows that the image of $c(a,b)$ is $([b]-[a])\zeta_p$: its even moments are $(1-p^{k-1})(a^k-b^k)B_k/k$. A choice of integer $e$ generating $\mathbb Z_p^\times$ topologically gives a norm-compatible generator $c(e,1)$, after multiplication by its constant [Teichmuller lift](../../../../../teichmuller-representative.md) to make it principal. That constant has zero logarithmic derivatives. Its conjugates generate the closed cyclotomic-unit module, and $[e]-[1]$ generates $I(G)$. This yields the displayed local quotient and its [characteristic ideal](../../../../../characteristic-ideal.md). The generation statement is an important ingredient; the mere calculation of a few moments would not prove the theorem.

The [class-field unit sequence](../../../../../class-field-unit-sequence.md) gives the global comparison

$$
0\longrightarrow B\longrightarrow H\longrightarrow X_\infty\longrightarrow Y_\infty\longrightarrow0,
\qquad B=E_\infty^1/C_\infty^1,\quad H=U_\infty^1/C_\infty^1.
$$

Multiplicativity of [characteristic ideals](../../../../../characteristic-ideal.md) in [exact sequences](../../../../../exact-sequence.md) gives

$$
\operatorname{char}(B)\operatorname{char}(X_\infty)
=\operatorname{char}(H)\operatorname{char}(Y_\infty).
$$

Thus the local theorem proves the main conjecture precisely when one proves **$\operatorname{char}(B)=\operatorname{char}(Y_\infty)$**. These terms measure the global-unit and ideal-class obstructions. Discarding them would silently impose a much stronger arithmetic hypothesis.

The first global step is the [Euler-system divisibility for real cyclotomic class modules](../../../../../euler-system-divisibility-for-real-cyclotomic-class-modules.md): a generator $f_Y$ of $\operatorname{char}(Y_\infty)$ divides a generator $f_B$ of $\operatorname{char}(B)$ on every character component. Here is the mechanism. Choose auxiliary primes $q$ splitting completely in a finite layer and satisfying $q\equiv1\pmod{p^m}$. For a generator $\sigma_q$ of its auxiliary cyclic group, put

$$
D_q=\sum_{i=1}^{q-2}i\sigma_q^i,\qquad
(\sigma_q-1)D_q=(q-1)-N_q.
$$

Apply products of these operators to the [unit](../../../../../unit-in-a-ring.md) [Cyclotomic Euler system](../../../../../cyclotomic-euler-system.md) of Question 3. The norm axiom and this group-ring identity make the derived elements invariant modulo $p^m$-th powers, so Kummer descent gives classes in $F_n^\times/(F_n^\times)^{p^m}$. The congruence axiom identifies the valuation at each newly introduced prime with a residue symbol of the preceding class; valuations away from the chosen auxiliary primes vanish modulo $p^m$. The [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md) supplies primes in prescribed ideal classes with the required residue-symbol behavior. Adding these primes successively forces the elementary divisors of the class group to divide the available cyclotomic-unit index. Taking the norm limit yields $f_Y\mid f_B$. Finite control defects do not survive localization at height-one primes; using two coprime annihilators of such a finite defect also shows that no hidden p-power factor is left. This is the substantive global argument furnished by the [Cyclotomic Euler system](../../../../../cyclotomic-euler-system.md), not a consequence of Iwasawa's local theorem alone.

For the reverse comparison use the [cyclotomic unit index formula](../../../../../cyclotomic-unit-index-formula.md) and norm descent, keeping invariants as well as coinvariants. At the base [field](../../../../../field.md) put $A_0$ for its p-primary [ideal class group](../../../../../ideal-class-group.md), and let $N_\infty(E_0^1)$ be the [universal norm of units in a Zp-extension](../../../../../universal-norm-of-units-in-a-zp-extension.md). Class-field and [unit](../../../../../unit-in-a-ring.md) descent, using total ramification and the principal prime over $p$, give

$$
Y_{\infty,\Gamma}\simeq A_0,\qquad
B_\Gamma\simeq N_\infty(E_0^1)/C_0^1,\qquad
\#(E_0^1/N_\infty(E_0^1))=\#Y_\infty^\Gamma.
$$

These are the required norm-defect control statements. The [cyclotomic unit index formula](../../../../../cyclotomic-unit-index-formula.md), with the p-adic closure justified by Leopoldt, gives $\#A_0=\#(E_0^1/C_0^1)$. Also $B^\Gamma=0$: its coinvariants are finite by the displayed control, so its invariants are finite by the [Iwasawa module structure theorem](../../../../../iwasawa-module-structure-theorem.md), whereas $B$ is a submodule of the cyclic local quotient $H$, which has no nonzero finite submodule. One must retain $Y_\infty^\Gamma$; dropping it would incorrectly identify all [global units](../../../../../global-unit-of-a-number-field.md) with universal norms.

Define the finite [Euler characteristic of a one-variable Iwasawa module](../../../../../euler-characteristic-of-a-one-variable-iwasawa-module.md) by $\chi_\Gamma(M)=\#M_\Gamma/\#M^\Gamma$. The preceding identities now give an exact cancellation:

$$
\chi_\Gamma(Y_\infty)
=\frac{\#(E_0^1/C_0^1)}{\#(E_0^1/N_\infty(E_0^1))}
=\#(N_\infty(E_0^1)/C_0^1)
=\chi_\Gamma(B).
$$

For a torsion $\Lambda$-module with finite invariant and coinvariant groups, the structure theorem gives $\chi_\Gamma(M)=|f_M(0)|_p^{-1}$. Write $f_{B,\chi}=f_{Y,\chi}h_\chi$ using the Euler-system divisibility. After forgetting $\Delta^+$, the [characteristic series](../../../../../characteristic-series-of-an-iwasawa-module.md) are the products of their character-component series. Equality of these [Euler characteristic of a one-variable Iwasawa module](../../../../../euler-characteristic-of-a-one-variable-iwasawa-module.md) values gives

$$
\sum_\chi v_p(h_\chi(0))=0.
$$

Every summand is nonnegative, since $h_\chi\in\mathbb Z_p[[S]]$. Each is therefore zero. A [formal power series](../../../../../formal-power-series.md) with p-adic-unit constant term is a [unit](../../../../../unit-in-a-ring.md), so every $h_\chi$ is a [unit](../../../../../unit-in-a-ring.md). Hence $\operatorname{char}(B)=\operatorname{char}(Y_\infty)$, and cancellation in the class-field [exact sequence](../../../../../exact-sequence.md) completes the boxed main conjecture.

The familiar reflected odd class-group formulation follows from [Kummer reflection in Iwasawa theory](../../../../../kummer-reflection-in-iwasawa-theory.md), with the inversion of the group variable and the [Tate twist](../../../../../tate-twist.md) both included. For example, for nontrivial even $\chi$, if $f_\chi((1+p)^s-1)=L_p(\chi,s)$, then the p-ramified series is $g_\chi(S)=f_\chi((1+p)(1+S)^{-1}-1)$, and $g_\chi((1+p)^{1-s}-1)=L_p(\chi,s)$. The proof above includes the exceptional trivial component through augmentation regularization. It assumes neither a vanishing real class group nor Vandiver's conjecture: the Euler-system divisibility and the norm-defect cancellation replace that extra hypothesis.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
