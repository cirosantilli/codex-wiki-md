<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $R$ is [reduced](../../../../reduced-ring.md), its [nilradical](../../../../nilradical.md) $N$ is zero. By [b](../b.md), every [localization at a prime ideal](../../../../localization-at-a-prime-ideal.md) has zero [nilradical](../../../../nilradical.md), so in particular $R_{\mathfrak m}$ is [reduced](../../../../reduced-ring.md) for every [maximal ideal](../../../../maximal-ideal.md) $\mathfrak m$.

Conversely, suppose every such [localization](../../../../localization-of-a-ring.md) is [reduced](../../../../reduced-ring.md). Take a [nilpotent element](../../../../nilpotent.md) $x\in R$. Then $x/1$ is [nilpotent](../../../../nilpotent.md) in every $R_{\mathfrak m}$, hence zero there. To see directly that $x=0$, suppose otherwise and consider the proper [annihilator](../../../../annihilator-ring-theory.md)

$$
\operatorname{Ann}_R(x)=\{a\in R:ax=0\}.
$$

Choose a [maximal ideal](../../../../maximal-ideal.md) $\mathfrak m$ containing this [annihilator](../../../../annihilator-ring-theory.md). The equality $x/1=0$ in $R_{\mathfrak m}$ would imply $sx=0$ for some $s\notin\mathfrak m$, by the [vanishing criterion in a module localization](../../../../vanishing-criterion-in-a-module-localization.md). But then $s\in\operatorname{Ann}_R(x)\subseteq\mathfrak m$, a contradiction. This is the principle that [localization detects zero elements](../../../../localization-detects-zero-elements.md). Therefore

$$
\boxed{R\text{ is reduced}\iff R_{\mathfrak m}\text{ is reduced for every maximal ideal }\mathfrak m.}
$$

The argument also includes the [zero ring](../../../../zero-ring.md), which is [reduced](../../../../reduced-ring.md) and has no [maximal ideals](../../../../maximal-ideal.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
