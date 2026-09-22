<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The construction must first specify the field of definition of the [complex multiplication](../../../../../complex-multiplication.md). Let $E/F$ be a [CM elliptic curve](../../../../../cm-elliptic-curve.md) and let $K$ be its geometric CM field, embedded by its action on an invariant differential. In characteristic zero this action is injective. Consequently every geometric [endomorphism](../../../../../endomorphism.md) is defined over $F'=FK$: a Galois automorphism fixing $FK$ fixes its differential scalar and therefore fixes the [endomorphism](../../../../../endomorphism.md) itself. Initially assume $F$ already contains $K$; we return to the other case below.

Choose a complex embedding and an analytic [complex uniformization of an elliptic curve](../../../../../complex-uniformization-of-an-elliptic-curve.md)

$$
E(\mathbb C)\simeq\mathbb C/L,\qquad L=\Omega\mathfrak a,
$$

where $\mathfrak a$ is a lattice in $K$, stable under the CM order $R$. It need not be the maximal order or a principal ideal. Its torsion is described by the finite adelic quotients of this lattice.

The input from the [CM reciprocity theorem](../../../../../cm-reciprocity-theorem.md) is precise: if $s$ is an idele of $F$, $n=N_{F/K}s$, and $\sigma=\operatorname{Art}_F(s)$, then $\sigma$ takes the CM torus to the torus with lattice $n_f^{-1}L$; on torsion the comparison is induced by multiplication by $n_f^{-1}$. This reciprocity statement comes from the ideal action on CM lattices: an ideal $\mathfrak b$ gives the isogeny to $\mathfrak b^{-1}L$, composition multiplies ideals, and adding torsion level structure removes automorphism ambiguity. The resulting action on algebraic CM points is the ray-class Artin action. This is the deep CM input, not an assertion that an arbitrary abelian [Galois representation](../../../../../galois-representation.md) automatically comes from an algebraic [Hecke character](../../../../../hecke-character.md).

Because $\sigma$ fixes $F$, the algebraic curve $E^\sigma$ is $E$. Comparing the reciprocity uniformization with the original one therefore gives multiplication by a scalar

$$
a(s_f)\in K^\times,\qquad a(s_f)n_f^{-1}L=L.
$$

The scalar belongs to $K$: a complex scalar carrying one lattice contained in $K$ to another is the quotient of two nonzero lattice elements. Its torsion action is

$$
\rho_\ell(\operatorname{Art}_F(s_f))=a(s_f)(N_{F/K}s_f)_\ell^{-1}\quad\text{in }(K\otimes\mathbb Q_\ell)^\times.
$$

The uniqueness of the torsion-compatible comparison is important: two possible scalars would induce the same action on all torsion, hence their difference would annihilate torsion of arbitrarily large order and be zero. Multiplying the torsion-action formulas for $s_f$ and $t_f$ now proves $a(s_ft_f)=a(s_f)a(t_f)$.

For $b\in F^\times$, [Artin reciprocity](../../../../../artin-reciprocity-law.md) sends its principal idele to the identity. The archimedean factors are complex and connected, so its finite part also has trivial Artin image. The preceding formula therefore gives

$$
a(b_f)=N_{F/K}(b).
$$

It follows that

$$
\boxed{\psi_E(s)=\frac{a(s_f)}{(N_{F/K}s)_\infty}}
$$

is trivial on principal ideles and defines a character of the [idèle class group](../../../../../idele-class-group.md) of $F$. This establishes the multiplicativity and principal-idele condition, rather than merely prescribing Frobenius values and hoping that they extend.

We must still prove continuity and a finite conductor. For a finite place $v$ and a prime $\ell$ different from its residue characteristic, an idele supported on the units at $v$ has trivial $\ell$-component of its norm. Thus its action on the [Tate module](../../../../../tate-module.md) is exactly multiplication by $a(u)$. At a place of [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md), inertia acts trivially, so $a(u)=1$. At a bad place, a CM curve has potentially good reduction, and inertia on the prime-to-residue-characteristic [Tate module](../../../../../tate-module.md) has finite image. Hence $a$ is trivial on an open subgroup of the local units there. There are only finitely many bad places. Together these facts give an open finite-congruence kernel on the unit ideles and prove continuity. The archimedean norm factor is already continuous. The potentially-good-reduction and inertia facts are the reduction-theoretic inputs in [Serre and Tate's treatment of CM abelian varieties](https://wstein.org/papers/bib/Serre-Tate-Good_Reduction_of_Abelian_Varieties.pdf).

Consequently $\psi_E$ is a [Hecke character](../../../../../hecke-character.md). In ideal notation, for $b\equiv1\pmod{\mathfrak f}$,

$$
\psi_E((b))=N_{F/K}(b),
$$

so its [infinity type of a Hecke character](../../../../../infinity-type-of-a-hecke-character.md) is the type determined by the chosen CM embedding, with the inverse archimedean norm in the idele convention. Nonmaximal orders merely contribute additional finite-level conditions; the proof retains their lattice and does not replace it by the maximal-order lattice without justification.

At a good prime $v$, choose a uniformizer idele and a prime $\ell$ different from the residue characteristic. Its norm has trivial $\ell$-component, so arithmetic Frobenius acts on the [Tate module](../../../../../tate-module.md) by $\psi_E(v)$. Specialization of prime-to-residue-characteristic torsion identifies this with the reduced [Frobenius isogeny](../../../../../frobenius-isogeny-of-an-elliptic-curve.md). Thus

$$
1-a_vT+Nv\,T^2=(1-\psi_E(v)T)(1-\overline{\psi_E(v)}T).
$$

The corresponding [Hasse-Weil L-function](../../../../../hasse-weil-l-function.md) factors as $L(E/F,s)=L(\psi_E,s)L(\bar\psi_E,s)$, including the local factors determined by inertia. This explains why the [Hecke character](../../../../../hecke-character.md) encodes both the torsion representations and the Euler factors.

If $F$ does not contain $K$, apply the construction over $FK$. The two conjugate CM characters are exchanged by the nontrivial automorphism of $FK/F$, and the two-dimensional [Galois representation](../../../../../galois-representation.md) over $F$ is their induced representation. In that case the natural description is $L(E/F,s)=L(\psi_E/FK,s)$ by induction, rather than a pair of one-dimensional characters over $F$. Question 3 supplies a concrete example: $\mathbb Q$ does not define $[i]$, whereas $\mathbb Q(i)$ does. This completes the existence argument for an arbitrary CM curve over a [number field](../../../../../number-field.md), with its field of definition correctly accounted for.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
