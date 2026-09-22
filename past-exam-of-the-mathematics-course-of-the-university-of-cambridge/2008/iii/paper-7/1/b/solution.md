<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The forward implication is immediate: the [localization of a module](../../../../../../localization-of-a-module.md) that is zero remains zero. Conversely, suppose $M\ne0$ and choose $0\ne x\in M$. Its [annihilator](../../../../../../annihilator-ring-theory.md)

$$
J=\operatorname{Ann}_A(x)=\{a\in A:ax=0\}
$$

is a proper [ideal](../../../../../../ideal.md), since $1\notin J$. Choose a [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$ containing $J$. Then $x/1$ cannot be zero in $M_{\mathfrak m}$: otherwise the [vanishing criterion in a module localization](../../../../../../vanishing-criterion-in-a-module-localization.md) would give $sx=0$ for some $s\notin\mathfrak m$, contradicting $s\in J\subseteq\mathfrak m$. Thus some maximal [localization](../../../../../../localization-of-a-ring.md) is nonzero, proving

$$
\boxed{M=0\iff M_{\mathfrak m}=0\text{ for every maximal ideal }\mathfrak m.}
$$

In the suggested cyclic description, $Ax\cong A/J$ and part (a) gives $(Ax)_{\mathfrak m}\ne0$; the same fraction argument embeds it in $M_{\mathfrak m}$. This is [localization detects zero elements](../../../../../../localization-detects-zero-elements.md), applied to an arbitrary [module](../../../../../../module-mathematics.md); finite generation is unnecessary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
