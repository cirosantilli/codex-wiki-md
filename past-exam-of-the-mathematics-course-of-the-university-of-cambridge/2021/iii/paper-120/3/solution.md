<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A partial function $f:\mathbb N^k\rightharpoonup\mathbb N$ is lambda-definable when a [lambda term](../../../../../lambda-term.md) $F$ sends the corresponding [Church numerals](../../../../../church-numeral.md) to the numeral for $f(\mathbf n)$ whenever the value is defined and produces no numeral otherwise; in other words, it is a [lambda-definable partial function](../../../../../lambda-definable-partial-function.md). The initial functions are represented by

$$
\mathbf 0=\lambda f.\lambda x.x,
\qquad
\operatorname{Succ}=\lambda n.\lambda f.\lambda x.f(nfx),
$$

and the appropriate variable in $\lambda x_1\ldots x_k.x_i$. If $G,H_1,\ldots,H_m$ represent $g,h_1,\ldots,h_m$, then

$$
\lambda\mathbf x.\,G(H_1\mathbf x)\cdots(H_m\mathbf x)
$$

represents their composition.

Church Booleans supply a lazy conditional, and

$$
\operatorname{IsZero}=\lambda n.\,n(\lambda x.\mathbf{False})\mathbf{True}
$$

tests whether a Church numeral is zero. A standard predecessor term is

$$
\operatorname{Pred}
=\lambda n.\lambda f.\lambda x.\,
n(\lambda g.\lambda h.\,h(gf))(\lambda u.x)(\lambda u.u).
$$

Let $G$ and $H$ represent the base and step functions of a primitive recursion. With a [fixed-point combinator](../../../../../fixed-point-combinator.md) $Y$, define

$$
R=Y\bigl(\lambda r.\lambda\mathbf x.\lambda n.\,
\operatorname{If}(\operatorname{IsZero}n)
(G\mathbf x)
(H\mathbf x(\operatorname{Pred}n)(r\mathbf x(\operatorname{Pred}n)))\bigr).
$$

Normal-order [beta reduction](../../../../../beta-reduction.md) evaluates only the selected branch. Induction on the input numeral gives the two recursion equations, so this is the [lambda definition of primitive recursion](../../../../../lambda-definition-of-primitive-recursion.md).

For [unbounded minimization](../../../../../mu-operator.md), let $G$ represent $g(\mathbf x,n)$ and define

$$
M=Y\bigl(\lambda r.\lambda\mathbf x.\lambda n.\,
\operatorname{If}(\operatorname{IsZero}(G\mathbf x n))
n
(r\mathbf x(\operatorname{Succ}n))\bigr).
$$

Then $M\mathbf x\mathbf0$ tests $0,1,2,\ldots$ in order and returns the least zero of $g$. If no zero is reached, or a required earlier computation is undefined, reduction never produces a Church numeral. This is the [lambda definition of unbounded minimization](../../../../../lambda-definition-of-unbounded-minimization.md). Since the partial recursive functions are generated from the initial functions by composition, primitive recursion, and minimization, every [partial computable function](../../../../../computable-function.md) is represented by a lambda term on Church numerals.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
