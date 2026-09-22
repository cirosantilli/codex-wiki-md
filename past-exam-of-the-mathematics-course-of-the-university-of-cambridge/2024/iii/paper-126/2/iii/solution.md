<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [finite complex computing cohomology in a proper flat family](../../../../../../finite-complex-computing-cohomology-in-a-proper-flat-family.md) gives a bounded complex $K^\bullet$ of finite locally free $A$-modules such that, for every $A$-module $M$,

$$
H^p(X,\mathcal F\otimes_AM)\simeq H^p(K^\bullet\otimes_AM).
$$

In particular, $M=A$ computes $H^p(X,\mathcal F)$ and $M=\kappa(s)$ computes $H^p(X_s,\mathcal F(s))$.

Since $H^p(K^\bullet)=0$ for $p>n$, the finite exact tail above degree $n$ can be split successively: its last differential is surjective onto a [projective module](../../../../../../projective-module.md), hence splits, and induction moves left. Removing the resulting contractible summands leaves a finite locally free complex ending in degree $n$. Therefore

$$
H^n(K^\bullet)=\operatorname{coker}(K^{n-1}\to K^n),
$$

and after tensoring with $\kappa(s)$ the same formula computes the fiber cohomology.

If $H^n(X,\mathcal F)=0$, the last differential is surjective, and remains so after every base change; hence every $H^n(X_s,\mathcal F(s))$ vanishes. Conversely, if all fiber groups vanish, the finitely generated cokernel $C$ satisfies $C\otimes_A\kappa(s)=0$ for every $s\in\operatorname{Spec}A$. Localizing and applying [Nakayama lemma](../../../../../../nakayama-lemma.md) gives $C_s=0$ for every $s$, so $C=0$. Thus

$$
\boxed{H^n(X,\mathcal F)=0\iff H^n(X_s,\mathcal F(s))=0\text{ for every }s\in\operatorname{Spec}A.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
