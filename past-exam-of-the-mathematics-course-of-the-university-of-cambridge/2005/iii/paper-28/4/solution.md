<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [global partial-fraction expansion of the zeta logarithmic derivative](../../../../../global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md), with zeros counted with multiplicity and paired summands retained, is

$$
\frac{\zeta'}{\zeta}(s)=B-\frac1s-\frac1{s-1}
+\frac12\log\pi-\frac12\frac{\Gamma'(s/2)}{\Gamma(s/2)}
+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right),
\qquad B=\frac{\xi'(0)}{\xi(0)}.
$$

For a nonprincipal [primitive Dirichlet character](../../../../../primitive-dirichlet-character.md) $\chi$ of [Dirichlet conductor](../../../../../conductor-of-a-dirichlet-character.md) $q$, put $a=0$ or $1$ according as $\chi(-1)=1$ or $-1$. Its [completed Dirichlet L-function](../../../../../completed-dirichlet-l-function.md) is

$$
\mathcal L_\chi(s)=\left(\frac q\pi\right)^{(s+a)/2}
\Gamma\left(\frac{s+a}{2}\right)L(s,\chi).
$$

The [global partial-fraction expansion of a Dirichlet L-function logarithmic derivative](../../../../../global-partial-fraction-expansion-of-a-dirichlet-l-function-logarithmic-derivative.md) is

$$
\boxed{\frac{L'}{L}(s,\chi)=B_\chi-\frac12\log\frac q\pi
-\frac12\frac{\Gamma'((s+a)/2)}{\Gamma((s+a)/2)}
+\sum_{\rho_\chi}\left(\frac1{s-\rho_\chi}+\frac1{\rho_\chi}\right),}
$$

where $B_\chi=\mathcal L_\chi'(0)/\mathcal L_\chi(0)$ and the zeros are the nontrivial zeros of the completion. These expansions follow from genus-one [Hadamard factorization](../../../../../hadamard-factorization-theorem.md); the combined terms converge locally normally. The primitive principal [Dirichlet character](../../../../../dirichlet-character.md) has [Dirichlet conductor](../../../../../conductor-of-a-dirichlet-character.md) one and gives the zeta formula. If a [Dirichlet character](../../../../../dirichlet-character.md) modulo $Q$ is induced by a [primitive Dirichlet character](../../../../../primitive-dirichlet-character.md) $\chi^*$ of [Dirichlet conductor](../../../../../conductor-of-a-dirichlet-character.md) $q$, its missing Euler factors add

$$
\sum_{\substack{p\mid Q\\p\nmid q}}
\frac{\chi^*(p)\log p}{p^s-\chi^*(p)}
$$

to the primitive [logarithmic derivative](../../../../../logarithmic-derivative.md). This correction is $O(\log Q)$ on the real interval $1<\sigma\leq2$.

The form needed here is [Landau theorem for two real Dirichlet characters](../../../../../landau-theorem-for-two-real-dirichlet-characters.md): there is an absolute $b>0$ such that, if $\chi_1,\chi_2$ are real primitive nonprincipal [Dirichlet characters](../../../../../dirichlet-character.md) of [Dirichlet conductors](../../../../../conductor-of-a-dirichlet-character.md) $q_1,q_2$ and their product is nonprincipal, then

$$
\boxed{L(s,\chi_1)L(s,\chi_2)\text{ has at most one real zero in }
1-\frac b{\log(q_1q_2)}<s<1,}
$$

counting multiplicity. In particular, two distinct primitive [real Dirichlet characters](../../../../../real-dirichlet-character.md) cannot each have a zero in that interval.

For the proof, induce the [Dirichlet characters](../../../../../dirichlet-character.md) to a common modulus and consider

$$
D(s)=\zeta(s)L(s,\chi_1)L(s,\chi_2)L(s,\chi_1\chi_2).
$$

The last factor can be imprimitive but is nonprincipal. For $\sigma>1$, logarithmic differentiation of the [Euler products](../../../../../euler-product.md) gives

$$
-\frac{D'}D(\sigma)=\sum_{n\geq1}
\frac{\Lambda(n)(1+\chi_1(n))(1+\chi_2(n))}{n^\sigma}\geq0.
$$

This positivity is the reason to include all four factors: each [real Dirichlet character](../../../../../real-dirichlet-character.md) takes values in $\{0,1,-1\}$, including at ramified [primes](../../../../../prime-number.md).

The real partial-fraction identity for a primitive completion has no residual real constant. Indeed, after taking real parts in its Hadamard derivative, the constant is determined to be zero by the functional-equation symmetry of its modulus across the critical line; the zero kernels there cancel in reflected pairs. Consequently

$$
\Re\frac{L'}L(s,\chi)
=\sum_{\rho_\chi}\Re\frac1{s-\rho_\chi}
-\frac12\log\frac q\pi
-\frac12\Re\frac{\Gamma'((s+a)/2)}{\Gamma((s+a)/2)}.
$$

For $1<\sigma\leq2$ all the zero kernels are nonnegative, and the gamma term is bounded. The missing Euler factors have the previously bounded correction. Combining the four [logarithmic derivatives](../../../../../logarithmic-derivative.md), and retaining any two candidate real zeros $\beta_1,\beta_2$ of $L(\chi_1)L(\chi_2)$, therefore gives

$$
0\leq-\frac{D'}D(\sigma)
\leq\frac1{\sigma-1}
-\frac1{\sigma-\beta_1}-\frac1{\sigma-\beta_2}
+C\log(q_1q_2).
$$

Zeros in any other factors only decrease this upper bound. The sole [pole](../../../../../pole.md) term comes from zeta.

Put $H=\log(q_1q_2)$ and choose $a>0$ so small that $Ca<1/10$. If both $1-\beta_j<a/(4H)$, take $\sigma=1+a/H$. The upper bound is then at most

$$
H\left(\frac1a-\frac2{a+a/4}+C\right)
=H\left(C-\frac3{5a}\right)<0,
$$

a contradiction. Taking $b=a/4$ proves the theorem, including the multiplicity assertion.

A [Siegel zero](../../../../../siegel-zero.md) is a possible exceptional real zero of the $L$-function of a real nonprincipal [primitive Dirichlet character](../../../../../primitive-dirichlet-character.md), in the very narrow zero-free-region exception near one. Fix a sufficiently small absolute threshold $\eta>0$ and call a zero exceptional here when

$$
1-\frac\eta{\log q}<\beta<1.
$$

Take $\eta<b/4$ and also smaller than the constant in the [classical zero-free region for Dirichlet L-functions](../../../../../classical-zero-free-region-for-dirichlet-l-functions.md). Such a zero, if present, is real and simple; its existence is not asserted. This choice fixes the constants consistently for the requested separation conclusions.

For two different real [primitive Dirichlet characters](../../../../../primitive-dirichlet-character.md) of the same modulus $q$, their product cannot be principal: otherwise they agree on all units and hence are the same [Dirichlet character](../../../../../dirichlet-character.md). Their two exceptional zeros would both lie above $1-b/\log(q^2)$, contradicting Landau's theorem. Thus **at most one real [primitive Dirichlet character](../../../../../primitive-dirichlet-character.md) modulo $q$ has an exceptional zero**.

For distinct primitive [Dirichlet conductors](../../../../../conductor-of-a-dirichlet-character.md) $q_1<q_2$, the product of their [Dirichlet characters](../../../../../dirichlet-character.md) is again nonprincipal; otherwise their common induced [Dirichlet character](../../../../../dirichlet-character.md) would have two different primitive [Dirichlet conductors](../../../../../conductor-of-a-dirichlet-character.md). Suppose $q_2\leq q_1^2$. Then

$$
\log(q_1q_2)\leq3\log q_1,\qquad
1-\beta_j<\frac\eta{\log q_j}\leq\frac\eta{\log q_1}
<\frac b{\log(q_1q_2)}\quad(j=1,2).
$$

Again both zeros violate the two-zero prohibition. Therefore the [sparse conductors of exceptional real Dirichlet zeros](../../../../../sparse-conductors-of-exceptional-real-dirichlet-zeros.md) obey

$$
\boxed{q_{j+1}>q_j^2.}
$$

The quadratic spacing uses a fixed sufficiently small exceptional-zero constant; it does not claim this conclusion for an arbitrarily enlarged neighbourhood of one.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
