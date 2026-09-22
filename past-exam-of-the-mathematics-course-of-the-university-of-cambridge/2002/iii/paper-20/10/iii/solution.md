<h1 id="10/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $(A,a)$, consider the [reflexive free-algebra presentation of a monad algebra](../../../../../../reflexive-free-algebra-presentation-of-a-monad-algebra.md)

$$
F^T(TA)\ \substack{\xrightarrow{\mu_A}\\[-2pt]\xrightarrow[T a]{}}\ F^T(A)\xrightarrow{a}(A,a).
$$

Both parallel [morphisms](../../../../../../morphism.md) are [monad algebra morphisms](../../../../../../morphism-of-algebras-for-a-monad.md): $\mu_A$ satisfies the [monad](../../../../../../monad.md) associativity law, while $Ta$ is the image under $F^T$ of $a$. The map $a$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) because $a\mu_A=aTa$, and the same equation says it equalizes the pair.

Suppose $h:F^T(A)\to(B,b)$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) with $h\mu_A=hTa$. Put $k=h\eta_A:A\to B$. [Naturality](../../../../../../naturality.md) of $\eta$ and the unit law give

$$
ka=h\eta_Aa=hTa\eta_{TA}=h\mu_A\eta_{TA}=h.
$$

Moreover, since $h$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md),

$$
bTk=bTh\,T\eta_A=h\mu_A T\eta_A=h=ka.
$$

Thus $k$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) and factors $h$ through $a$. If $k'a=h$, then $k'=k'a\eta_A=h\eta_A=k$, proving uniqueness. Therefore **every [monad](../../../../../../monad.md) algebra is the stated [coequalizer](../../../../../../coequalizer.md) of free algebras**.

The underlying fork is a [split coequalizer](../../../../../../split-coequalizer.md): take $q=a$, $s=\eta_A$ and $t=\eta_{TA}$. Then $qs=1_A$, $\mu_A t=1_{TA}$, and $(Ta)t=sa$. Its splitting maps need not be [monad algebra morphisms](../../../../../../morphism-of-algebras-for-a-monad.md); the preceding argument separately proves the [coequalizer](../../../../../../coequalizer.md) in $\mathcal C^T$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [10](../../10.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
