<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $F:\mathcal C\rightleftarrows\mathcal D:G$ with $F\dashv G$, the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md) is $T=GF$, with unit the adjunction unit and multiplication $\mu=G\varepsilon F$. An [algebra for a monad](../../../../../algebra-for-a-monad.md) is a map $a:TA\to A$ satisfying $a\eta_A=1_A$ and $aT(a)=a\mu_A$. The [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) is

$$
K:\mathcal D\to\mathcal C^T,
\qquad K(D)=(GD,G\varepsilon_D),
$$

and sends a morphism $h$ to $Gh$.

Given a $T$-algebra $(A,a)$, form in $\mathcal D$ the coequalizer

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA
\longrightarrow J(A,a).
$$

The pair is reflexive, with common section $F\eta_A$, so it exists by hypothesis. A map $J(A,a)\to D$ is equivalently a map $FA\to D$ equalizing the pair. Under adjunction this is exactly a map $A\to GD$ satisfying the $T$-algebra homomorphism equation. Hence

$$
\mathcal D(J(A,a),D)\cong\mathcal C^T((A,a),K(D)),
$$

naturally, and $J\dashv K$. Iterating these comparison adjunctions gives the monadic tower; the [monadic length](../../../../../monadic-length.md) is the least number of steps required to reach an equivalence.

For a pair of sets $(X_0,X_1)$, define

$$
F(X_0,X_1)=\bigl(X_0\hookrightarrow X_0\sqcup X_1\bigr).
$$

A pair of maps $X_0\to A_0$, $X_1\to A_1$ extends uniquely to a commutative square from this inclusion to any injection $A_0\hookrightarrow A_1$, proving that $F$ is left adjoint to the forgetful functor $U:\mathbf{Mono(Set)}\to\mathbf{Set}\times\mathbf{Set}$.

The induced monad sends $(X_0,X_1)$ to $(X_0,X_0\sqcup X_1)$. Its algebra unit laws show that an algebra is precisely an arbitrary function $X_0\to X_1$, with no injectivity requirement. Thus its [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) is the arrow category $[\mathbf2,\mathbf{Set}]$, and the comparison functor is the full inclusion of injections into all functions. This inclusion is not an equivalence, so the original adjunction is not monadic. It is reflective: a function $f:A_0\to A_1$ maps to its image inclusion $\operatorname{im}f\hookrightarrow A_1$. The supplied result that reflections are monadic says that the next comparison is an equivalence. Therefore the original adjunction has monadic length $2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
