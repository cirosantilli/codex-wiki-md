<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [smooth projective curve](../../../../../../smooth-projective-curve.md) $C$ of [geometric genus](../../../../../../geometric-genus.md) one, the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) says

$$
\ell(D)-\ell(K_C-D)=\deg D.
$$

The [canonical divisor](../../../../../../canonical-divisor.md) has degree zero and is principal because a nonzero regular differential has no zeros. Hence $K_C\sim0$, so equivalently

$$
\ell(D)-\ell(-D)=\deg D.
$$

In particular, $\ell(D)=\deg D$ when $\deg D>0$.

The group $\operatorname{Pic}^0(E)$ is the group of degree-zero [divisor classes](../../../../../../divisor-class.md) on $E$, with addition induced by addition of divisors. Consider

$$
\iota:E\longrightarrow\operatorname{Pic}^0(E),
\qquad P\longmapsto[(P)-(O_E)].
$$

For surjectivity, let $D$ have degree zero. Since $\deg(D+(O_E))=1$, Riemann--Roch gives $\ell(D+(O_E))=1$. A nonzero element of this space makes $D+(O_E)$ linearly equivalent to an effective divisor of degree one, necessarily $(P)$ for some point $P$. Thus $[D]=[(P)-(O_E)]$.

For injectivity, suppose $(P)-(O_E)$ is a [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md). If $P\ne O_E$, its defining function would be nonconstant and would have at most one simple pole, whereas Riemann--Roch gives $\ell((O_E))=1$, so every such function is constant. Therefore $P=O_E$, and $\iota$ is a bijection.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
