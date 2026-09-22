<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [algebra for a monad](../../../../../../algebra-for-a-monad.md) $(A,a)$, consider the fork in the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md)

$$
\boxed{F(TA)\ \mathrel{\substack{\xrightarrow{\ \mu_A\ }\\[-2pt]\xrightarrow[\ Ta\ ]{}}}\ F(A)\xrightarrow{\ a\ }(A,a).}
$$

Here $\mu_A:F(TA)\to F(A)$ is the counit at $F(A)$, and $Ta=F(a)$. The arrow $a$ is an algebra morphism by $a\mu_A=aTa$, which also says that it coequalizes the two arrows.

Let $h:F(A)\to(B,b)$ be an algebra morphism with $h\mu_A=hTa$. Define $g=h\eta_A:A\to B$. Naturality of $\eta$ at $a$ gives

$$
ga=h\eta_Aa=hTa\,\eta_{TA}=h\mu_A\eta_{TA}=h.
$$

Since $h$ is an algebra morphism,

$$
bTg=bTh\,T\eta_A=h\mu_A T\eta_A=h=ga.
$$

Thus $g:(A,a)\to(B,b)$ is an algebra morphism with $ga=h$. Any other such factorization satisfies $g'=g'a\eta_A=h\eta_A=g$. This proves the full [coequalizer](../../../../../../coequalizer.md) universal property inside the algebra category.

The pair is moreover a [reflexive pair](../../../../../../reflexive-pair.md): its common section is $F(\eta_A)$, with underlying map $T\eta_A$, because $\mu_AT\eta_A=1_{TA}$ and $Ta\,T\eta_A=T(a\eta_A)=1_{TA}$. Hence **every monad algebra is a reflexive coequalizer of free algebras**. This [reflexive free-algebra presentation of a monad algebra](../../../../../../reflexive-free-algebra-presentation-of-a-monad-algebra.md) needs no general existence theorem for arbitrary algebra-category colimits.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
