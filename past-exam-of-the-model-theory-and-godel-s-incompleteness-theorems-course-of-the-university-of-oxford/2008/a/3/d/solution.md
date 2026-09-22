<h1 id="a/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $j=i+n$ with $n\ge1$. [Positive introspection](../../../../../positive-introspection.md) supplies the theorem $F_k\to F_{k+1}$ for every $k\ge1$, since $F_k$ itself has the form $P_S(\ulcorner F_{k-1}\urcorner)$.

[Induction](../../../../../mathematical-induction.md) on $n$ consequently gives

$$
S\vdash F_{i+1}\to F_{i+n}.
$$

At $n=1$ this is the identity implication. To pass from $n$ to $n+1$, compose the [induction](../../../../../mathematical-induction.md) hypothesis with the positive-introspection implication at $k=i+n$, which is at least one. Composing the result with the assumed $F_j\to F_i$ gives

$$
S\vdash F_{i+1}\to F_i,
$$

i.e. $S\vdash P_S(\ulcorner F_i\urcorner)\to F_i$. Löb's rule now yields

$$
\boxed{S\vdash F_i.}
$$

The index restriction on [positive introspection](../../../../../positive-introspection.md) has been respected even when $i=0$: the chain begins at $F_{i+1}$, which already is a provability assertion.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
