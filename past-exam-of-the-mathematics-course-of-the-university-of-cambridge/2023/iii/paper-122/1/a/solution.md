<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In an independent Bernoulli product space, an event is [increasing](../../../../../../increasing-event.md) if changing any coordinate from $0$ to $1$ cannot destroy it. [Harris' inequality](../../../../../../harris-inequality.md) says that two increasing events $A,B$ satisfy

$$
\mathbb P(A\cap B)\geq\mathbb P(A)\mathbb P(B).
$$

Equivalently, two decreasing events are positively correlated.

For [Janson inequalities](../../../../../../janson-inequality.md), let $R$ be a random subset of a finite ground set whose elements are selected independently, let $(S_i)_{i\in I}$ be fixed subsets, and put

$$
I_i=\mathbf1_{\{S_i\subseteq R\}},\qquad
X=\sum_i I_i,\qquad
\mu=\mathbb EX.
$$

Write $i\sim j$ when $i\ne j$ and $S_i\cap S_j\ne\varnothing$, and define the ordered dependency sum

$$
\Delta=\sum_{i\sim j}\mathbb E(I_iI_j).
$$

The first Janson inequality is

$$
\mathbb P(X=0)\leq\exp\left(-\mu+\frac{\Delta}{2}\right).
$$

The usual extended form is

$$
\mathbb P(X=0)
\leq
\begin{cases}
e^{-\mu/2},&\Delta\leq\mu,\\
e^{-\mu^2/(2\Delta)},&\Delta\geq\mu.
\end{cases}
$$

There is also the complementary lower bound

$$
\mathbb P(X=0)\geq\prod_i(1-\mathbb EI_i),
$$

and if $\mathbb EI_i\leq\varepsilon<1$ for all $i$, the product is at least $\exp(-\mu/(1-\varepsilon))$.

For the proof, order $I$ arbitrarily and expose the avoidance events one at a time. The standard [Janson sequential product lemma](../../../../../../janson-sequential-product-lemma.md), obtained by conditioning and using Harris' inequality on the coordinates outside $S_i$, gives

$$
\mathbb P(X=0)
\leq
\prod_i\left(1-\mathbb EI_i+sum_{j<i:j\sim i}\mathbb E(I_iI_j)\right).
$$

Using $1-x\leq e^{-x}$ and summing the pair terms yields $e^{-\mu+\Delta/2}$. If $\Delta\leq\mu$, this is at most $e^{-\mu/2}$. If $\Delta>\mu$, adjoin an independent Bernoulli coordinate of mean $q=\mu/\Delta$ to each index and intersect $A_i$ with the event that its new coordinate is $1$. The event $X=0$ implies that none of these thinned events occurs, while the thinned family has mean $q\mu$ and dependency sum $q^2\Delta$. Applying the first inequality in the enlarged product space gives

$$
\mathbb P(X=0)leq
\exp\left(-q\mu+\frac{q^2\Delta}{2}\right)
=e^{-\mu^2/(2\Delta)}.
$$

Finally, the events $I_i=0$ are decreasing, so repeated [Harris' inequality](../../../../../../harris-inequality.md) proves the product lower bound; $log(1-x)\geq-x/(1-\varepsilon)$ gives its exponential version.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
