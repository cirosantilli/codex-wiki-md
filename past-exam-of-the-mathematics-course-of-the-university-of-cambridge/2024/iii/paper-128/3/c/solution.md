<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conditions in $G$ are compatible finite functions, so their union $F=\bigcup G$ is a function $(\omega_1)^M\rightharpoonup(\omega_1)^M$. For each $\alpha<\omega_1$, the set

$$
D_\alpha=\{p:\alpha\in\operatorname{dom}p\}
$$

is dense: choose a normal function extending $p$ and add its value at $\alpha$. Genericity makes $F$ total.

If $\alpha<\beta$, choose a condition in the filter extending conditions that decide both values. It is contained in a [normal function on an ordinal](../../../../../../normal-function-on-an-ordinal.md), so $F(\alpha)<F(\beta)$. Thus $F$ is strictly increasing.

It remains to prove continuity. For every limit $\delta<\omega_1$ and $\gamma<\omega_1$, let $D_{\delta,\gamma}$ contain the conditions $p$ such that $\delta\in\operatorname{dom}p$ and either

$$
p(\delta)\le\gamma
$$

or there is some $\alpha<\delta$ in $\operatorname{dom}p$ with $p(\alpha)>\gamma$. This set is dense. Given $p$, extend it to a normal function $f$ and add $(\delta,f(\delta))$; if $f(\delta)>\gamma$, continuity of $f$ supplies an $\alpha<\delta$ with $f(\alpha)>\gamma$, which may also be added.

Now fix $\gamma<F(\delta)$. Since $G$ meets $D_{\delta,\gamma}$, compatibility with the condition deciding $F(\delta)$ rules out the first alternative and gives $\alpha<\delta$ with $F(\alpha)>\gamma$. Therefore values below $\delta$ are cofinal in $F(\delta)$. Strict increase supplies the reverse bound, so

$$
\boxed{F(\delta)=\sup_{\alpha<\delta}F(\alpha).}
$$

**Hence $F$ is normal on $(\omega_1)^M$ in $M[G]$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 128](../../../paper-128-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
