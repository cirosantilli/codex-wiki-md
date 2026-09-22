<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put every [formal pseudodifferential operator](../../../../../../formal-pseudodifferential-operator.md) in normal order, with all [coefficient](../../../../../../coefficient.md) [functions](../../../../../../function-split.md) on the left. Its [formal pseudodifferential residue](../../../../../../formal-pseudodifferential-residue.md) is the [coefficient](../../../../../../coefficient.md) of $\partial^{-1}$. The [Adler trace](../../../../../../adler-trace.md) is

$$
\boxed{\operatorname{Tr}P=\int\operatorname{res}P\,dx.}
$$

Here and below, use periodic [coefficients](../../../../../../coefficient.md) and integrate over a period, or impose convergence and vanishing boundary terms on the real line. Equivalently, the algebraic integration [functional](../../../../../../functional.md) must annihilate total [derivatives](../../../../../../derivative.md). This convention is needed for the requested trace property; arbitrary elements of $C^\infty(\mathbb R)$ do not supply it automatically.

It suffices to compute with monomials $A=a\partial^p$, $B=b\partial^q$. Write $r=p+q+1$. If $r<0$, no term in either product has power $\partial^{-1}$, so both residues are zero. If $r\geq0$, the [formal pseudodifferential composition rule](../../../../../../formal-pseudodifferential-composition-rule.md) gives

$$
\operatorname{res}(AB)=\binom pr a b^{(r)},\qquad
\operatorname{res}(BA)=\binom qr b a^{(r)}.
$$

Since $q=r-1-p$, reversal of the factors in the numerator proves

$$
\binom qr=\frac{(r-1-p)\cdots(-p)}{r!}=(-1)^r\binom pr.
$$

After $r$ integrations by parts, $\int ab^{(r)}dx=(-1)^r\int ba^{(r)}dx$. Hence the two product traces agree. More explicitly, for $r\geq1$ their residue difference is the total [derivative](../../../../../../derivative.md)

$$
\operatorname{res}[A,B]
=\binom pr\frac{d}{dx}\left(\sum_{j=0}^{r-1}(-1)^j a^{(j)}b^{(r-1-j)}\right).
$$

For $r=0$ the residue difference is $ab-ba=0$. In products of operators bounded above in order, only finitely many monomial pairs can contribute to a residue: the required $r$ is nonnegative, so the two downward [coefficient](../../../../../../coefficient.md) indices have a bounded sum. Summing the monomial result therefore proves

$$
\boxed{\operatorname{Tr}[P_1,P_2]=0,\qquad
\operatorname{Tr}(P_1P_2)=\operatorname{Tr}(P_2P_1).}
$$

The boundary convention is substantive. Without it, take $A=\partial^2$, $B=(\tanh x)\partial^{-2}$. Both individual residues vanish, but $\operatorname{res}[A,B]=2(\tanh x)'=2\operatorname{sech}^2x$ and its integral over $\mathbb R$ is $4$, not zero. The primitive has unequal limits at the two ends. Also a generic smooth residue need not have a convergent integral at all. Thus the proof supplies the intended cyclic trace under its necessary analytic or formal integration convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
