<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the simple-root form of [Hensel lemma](../../../../../../hensel-s-lemma.md). Let $R$ be a [complete discrete valuation ring](../../../../../../complete-discrete-valuation-ring.md), let $\pi$ be a [uniformizer](../../../../../../uniformizer.md), and let $F\in R[T]$. If $\bar a\in R/(\pi)$ is a root of $\bar F$ with $\bar F'(\bar a)\ne0$, then **there is exactly one root $a\in R$ reducing to $\bar a$.**

Choose a lift $a_1$ of $\bar a$. Suppose $F(a_r)\in\pi^rR$. To construct a lift satisfying the next congruence, write $a_{r+1}=a_r+\pi^r t_r$. The [polynomial](../../../../../../polynomial-split.md) expansion gives

$$
F(a_r+\pi^r t_r)\equiv F(a_r)+\pi^r t_rF'(a_r)\pmod{\pi^{r+1}}.
$$

Since $F'(a_r)$ is a [unit](../../../../../../unit-in-a-ring.md), its residue is invertible in the [residue field](../../../../../../residue-field.md). There is a unique residue class of $t_r$ making this zero modulo $\pi^{r+1}$. Thus $a_{r+1}\equiv a_r\pmod{\pi^r}$ and $F(a_{r+1})\equiv0\pmod{\pi^{r+1}}$. This produces a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the [complete discrete valuation ring](../../../../../../complete-discrete-valuation-ring.md). Its limit $a$ satisfies $F(a)=0$ by [continuity](../../../../../../continuous-function.md) of [polynomial](../../../../../../polynomial-split.md) evaluation, and $a\equiv a_1\pmod\pi$.

For uniqueness, suppose $a,b$ are two such roots. Polynomial division of their difference gives

$$
F(b)-F(a)=(b-a)\bigl(F'(a)+(b-a)H(a,b)\bigr),\qquad H\in R[S,T].
$$

Because $b-a\in\pi R$, the second factor is a [unit](../../../../../../unit-in-a-ring.md). Hence $b-a=0$. The simple-root hypothesis is used both for constructing successive lifts and for this uniqueness argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
