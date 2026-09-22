<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $f$ is [injective](../../../../../../injective-function.md). If $f_{\mathfrak m}(x/s)=0$, some $t\notin\mathfrak m$ satisfies $tf(x)=f(tx)=0$. Injectivity gives $tx=0$, and the [vanishing criterion in a module localization](../../../../../../vanishing-criterion-in-a-module-localization.md) gives $x/s=0$. Hence every localized [module homomorphism](../../../../../../module-homomorphism.md) is [injective](../../../../../../injective-function.md).

Conversely, suppose all $f_{\mathfrak m}$ are [injective](../../../../../../injective-function.md). For $x\in\ker f$, its image $x/1$ in $M_{\mathfrak m}$ maps to zero and therefore is zero for every [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$. The [annihilator](../../../../../../annihilator-ring-theory.md) argument in part (b) implies $x=0$. Thus $\ker f=0$ and $f$ is [injective](../../../../../../injective-function.md). We have proved that [injectivity of a module map is detected at maximal localizations](../../../../../../injectivity-of-a-module-map-is-detected-at-maximal-localizations.md):

$$
\boxed{f\text{ injective}\iff f_{\mathfrak m}\text{ injective for every maximal }\mathfrak m.}
$$

Equivalently, [exactness of localization](../../../../../../exactness-of-localization.md) gives $(\ker f)_{\mathfrak m}\cong\ker(f_{\mathfrak m})$, and part (b) detects whether this [kernel](../../../../../../kernel-of-a-linear-map.md) is zero.

## ↑ Ancestors (11)

1. [C](../c.md)
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
